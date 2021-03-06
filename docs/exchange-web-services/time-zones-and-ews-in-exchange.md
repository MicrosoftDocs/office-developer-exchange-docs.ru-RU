---
title: Часовые пояса и EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Узнайте, как часовые пояса работают с управляемым API EWS и EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 8435087d7709b77e7562e2b9d50ece58377dd8db
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463750"
---
# <a name="time-zones-and-ews-in-exchange"></a>Часовые пояса и EWS в Exchange

Узнайте, как часовые пояса работают с управляемым API EWS и EWS в Exchange.
  
Часовые пояса — это не то, что большинство людей придумало. Тем не менее, это важный принцип при указании дат и времени с помощью управляемого API EWS или EWS. Неправильное обработку часовых поясов в управляемом API EWS или приложении EWS может привести к непредвиденным результатам. Правильное управление часовыми поясами очень просто, если вы знаете, как.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Обработка часовых поясов в управляемом API EWS

Если вы используете управляемый API EWS, часовые пояса для большей части, которые обрабатываются автоматически. Без явного действия с вашей частью API использует местный часовой пояс клиентского компьютера и обрабатывает все необходимые преобразования в фоновом режиме. Это очень удобно, если это желаемый эффект, но у вас есть и другие варианты.
  
Один из вариантов — установка свойства [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Это свойство управляет часовым поясом для всех запросов, выполняемых управляемым API EWS. Это свойство доступно только для чтения; единственный способ задать его с помощью конструктора класса. При использовании конструктора [ExchangeService (System. тимезонеинфо)](https://msdn.microsoft.com/library/dd635875%28v=exchg.80%29.aspx) или [ExchangeService (ексчанжеверсион, System. тимезонеинфо)](https://msdn.microsoft.com/library/dd636248%28v=exchg.80%29.aspx) можно указать определенный часовой пояс как объект [System. тимезонеинфо](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx) . Если вы используете один из других конструкторов, не использующих объект **тимезонеинфо** в качестве параметра, класс **ExchangeService** устанавливает свойство **TimeZone** в текущий часовой пояс клиентского компьютера. 
  
Если вы задаете определенный часовой пояс или оставляете его в качестве часового пояса клиентского компьютера, все даты и время выражаются в часовом поясе, представленном свойством **TimeZone** . Управляемый API EWS предоставляет все свойства даты и времени как структуры [System. DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx) . Таким образом, если вы задаете свойства даты и времени, осторожным, что указанное время интерпретируется в соответствии со значением свойства [DateTime. Kind](https://msdn.microsoft.com/library/system.datetime.kind%28v=vs.110%29.aspx) для объекта **DateTime** . Если свойству **Kind** присвоено значение не **указано**, то значение **DateTime** интерпретируется как настраивается в часовом поясе, указанном в свойстве **TimeZone** . При чтении свойств даты/времени все свойства **DateTime** выражаются в этом часовом поясе. 
  
Если вы [создаете новые встречи или собрания](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) или [обновляете существующие встречи или собрания](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), вы можете переопределить часовой пояс, указанный в **часовом поясе** для новых объектов [встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) . Тем не менее, именно то, что можно переопределить, зависит от целевой [версии схемы EWS](ews-schema-versions-in-exchange.md) . Для всех значений свойства [ExchangeService. рекуестедсерверверсион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) можно задать значение свойства Meeting [. StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) , чтобы использовать конкретный часовой пояс для встречи или собрания. Если вы используете значение для свойства **ExchangeService. рекуестедсерверверсион** , которое больше **Exchange2007_SP1**, можно также задать свойство [встреча. EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , позволяющее указать часовой пояс для свойства [встреча. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) . Однако помните, что эти свойства влияют только на интерпретацию даты и времени для запроса на создание. Если вы получаете встречу, время начала и окончания по-прежнему будет выражаться в часовом поясе, указанном в свойстве **TimeZone** . 
  
Если вы обновляете существующие встречи или собрания, вы можете изменить часовой пояс для объекта **встречи** , задав свойство **StartTimeZone** и/или свойство **EndTimeZone** . Это приведет к соответствующим сдвигам времени. Если для свойства **ExchangeService. рекуестедсерверверсион** задано значение **Exchange2007_SP1**, невозможно задать свойство **EndTimeZone** ; на месте будет использоваться значение свойства **StartTimeZone** . 
  
**Таблица 1. Свойства часового пояса в управляемом API EWS**

|**Свойство часового пояса**|**Минимальная версия запроса сервера**|**Описание**|
|:-----|:-----|:-----|
|[Часовой](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Если не задано с помощью конструктора для класса **ExchangeService** , для этого свойства задается часовой пояс клиентского компьютера. Все свойства **DateTime** при создании элементов и при извлечении существующих элементов выражаются в этом часовом поясе. Этот часовой пояс можно переопределить в запросах на создание встреч и собраний, задав свойство Meeting **. StartTimeZone** и/или свойство **встреча. EndTimeZone** . Если свойство **встреча. StartTimeZone** не переопределяется, этот часовой пояс считается часовым поясом создания встреч и собраний.  <br/> |
|[StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Если для новых объектов **встреча** задано значение, этот часовой пояс используется для интерпретации свойств [встреча. Start](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) и [встреча. реминдердуеби](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Этот часовой пояс также учитывается в качестве часового пояса для объекта " **встреча** ".  <br/> При получении существующих элементов это свойство предназначено только для информационных целей. Значения свойств **DateTime** в существующей встрече всегда выражаются в часовом поясе, указанном в свойстве **ExchangeService. TimeZone** .  <br/> |
|[EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |Если для новых объектов **встреча** задано значение, этот часовой пояс используется для интерпретации свойства [встреча. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> При получении существующих элементов это свойство предназначено только для информационных целей. Значения свойств **DateTime** в существующей встрече всегда выражаются в часовом поясе, указанном в свойстве **ExchangeService. TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Обработка часовых поясов в EWS

Если вы используете EWS, то Часовые пояса не будут обрабатываться автоматически, а все еще сложнее. Влияние часовых поясов на запросы и ответы EWS зависит от ряда факторов.
  
- Версия Exchange, указанная в элементе [рекуестсерверверсион](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- Часовой пояс, указанный в элементе [тимезонеконтекст](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (при наличии) 
    
- Часовой пояс, указанный в элементах [митингтимезоне](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)или [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (если он присутствует в встречах или собраниях). 
    
- Часовой пояс, указанный в элементах **DateTime** XML (при наличии) 
    
В часовом поясе, указанном в значении элементов **DateTime** , может быть три формы. Вы можете прочитать все сведения в [схеме XML Part 2: Types Second Edition](http://www.w3.org/TR/xmlschema-2/#dateTime), а не в фразой:
  
- Всеобщее **скоординированное время (UTC):** Задается "Z". Например,  `2014-06-06T19:00:00.000Z`.
    
- **Конкретный часовой пояс:** Задается символами "+" или "–", за которыми следуют часы и минуты. Например,  `2014-06-06T19:00:00.000-08:00`.
    
- **Без часового пояса:** Задается отсутствием любого часового пояса. Например,  `2014-06-06T19:00:00.000`.
    
Если часовой пояс присутствует в значении **DateTime** (UTC или определенном часовом поясе), это значение всегда интерпретируется как часовой пояс. Если часовой пояс отсутствует, интерпретация значения зависит от конкретного сочетания других элементов, связанных с часовым поясом. 
  
**Таблица 2. Элементы часовых поясов в EWS и их последствиях**

|**рекуестсерверверсион**|**Присутствует Тимезонеконтекст?**|**Митингтимезоне, StartTimeZone или EndTimeZone присутствует (только для Календаритем и свойство meetingrequest)?**|**Дата и время в формате UTC**|**Дата и время в определенном часовом поясе**|**Дата и время без часового пояса**|**Часовой пояс создания встреч и собраний**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Да  <br/> |Да ( **митингтимезоне** )  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Элементы в элементе [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [свойство meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) , содержащие элемент **митингтимезоне** , интерпретируются как часовой пояс в элементе **митингтимезоне** , все остальные интерпретируются как время в формате UTC.  <br/> |Часовой пояс в элементе **митингтимезоне**  <br/> |
|**Exchange2007_SP1** <br/> |Да  <br/> |Нет  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Интерпретируется как время в формате UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Нет  <br/> |Да ( **митингтимезоне** )  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Элементы в элементе [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [свойство meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) , содержащие элемент **митингтимезоне** , интерпретируются как часовой пояс в элементе **митингтимезоне** , все остальные интерпретируются как время в формате UTC.  <br/> |Часовой пояс в элементе **митингтимезоне**  <br/> |
|**Exchange2007_SP1** <br/> |Нет  <br/> |Нет  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Интерпретируется как время в формате UTC  <br/> |UTC  <br/> |
|**Exchange2010** и более поздние версии  <br/> |Да  <br/> |Да ( **StartTimeZone** и/или **EndTimeZone** )  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Если присутствует элемент **StartTimeZone** , то значение элементов [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [реминдердуеби](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) интерпретируется как часовой пояс в элементе **StartTimeZone** . В противном случае значение этих элементов интерпретируется как часовой пояс в элементе **тимезонеконтекст** .  <br/> Если присутствует элемент **EndTimeZone** , значение [начального](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) элемента интерпретируется как часовой пояс в элементе **EndTimeZone** . В противном случае значение **End** элемента интерпретируется как часовой пояс в элементе **тимезонеконтекст** .  <br/> Элементы, не входящие в состав [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [свойство meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) , интерпретируются как часовой пояс в элементе **тимезонеконтекст** .  <br/> |Часовой пояс в элементе **StartTimeZone** , если он указан, то есть часовой пояс в элементе **тимезонеконтекст** , если нет  <br/> |
|**Exchange2010** и более поздние версии  <br/> |Да  <br/> |Нет  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Интерпретируется как часовой пояс в элементе **тимезонеконтекст**  <br/> |Часовой пояс в элементе **тимезонеконтекст**  <br/> |
|**Exchange2010** и более поздние версии  <br/> |Нет  <br/> |Да ( **StartTimeZone** и/или **EndTimeZone** )  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Если присутствует элемент **StartTimeZone** , то значение элементов [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и [реминдердуеби](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) интерпретируется как часовой пояс в элементе **StartTimeZone** . В противном случае значение этих элементов интерпретируется как время в формате UTC.  <br/> Если присутствует элемент **EndTimeZone** , значение [начального](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) элемента интерпретируется как часовой пояс в элементе **EndTimeZone** . В противном случае значение **конечного** элемента интерпретируется как время в формате UTC.  <br/> Элементы, не входящие в состав [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [свойство meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) , интерпретируются как время в формате UTC.  <br/> |Часовой пояс в элементе **StartTimeZone** , если он есть, в формате UTC, если нет  <br/> |
|**Exchange2010** и более поздние версии  <br/> |Нет  <br/> |Нет  <br/> |Интерпретируется как время в формате UTC  <br/> |Интерпретируется как часовой пояс, указанный в значении  <br/> |Интерпретируется как время в формате UTC  <br/> |UTC  <br/> |
   
При интерпретации ответов с сервера следует всегда проверять значение каждого элемента и соответствующим образом интерпретировать значение. Exchange всегда будет включать часовой пояс (UTC или конкретный часовой пояс) в значение.
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Дополнительные сведения о часовом поясе при создании встреч и собраний

При создании встречи или собрания часовой пояс, который применяется к времени начала, считается часовым поясом создания встречи. В дополнение к управлению интерпретацией даты и времени при создании встречи или собрания, в этом элементе отображается указанный ниже эффект.
  
- Если элемент является событием на целый день, он может отображаться непредвиденным образом при просмотре из клиента, который использует другой часовой пояс, чем часовой пояс создания. Это связано с тем, что [при создании события на целый день](how-to-create-all-day-events-by-using-ews-in-exchange.md)время начала и окончания каждого события на целый день регулируется до полуночи часового пояса для создания. Это время будет показываться как время, отличное от полуночи, в другом часовом поясе, поэтому элемент может оказаться в занимать дополнительные дни. Поэтому мы рекомендуем использовать часовой пояс, настроенный для основного клиента календаря пользователя, чтобы создать события на целый день, когда это возможно.
    
- Если элемент является собранием, часовой пояс создания будет отображаться на панели информации Outlook на приглашениях на собрания, получаемых участниками, если этот часовой пояс отличается от часового пояса клиента.
    
## <a name="in-this-section"></a>В этой статье

- [Создание встречи в определенном часовом поясе с помощью EWS в Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Обновление часового пояса встречи с помощью EWS в Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Версии схемы EWS в Exchange](ews-schema-versions-in-exchange.md)
    
- [Создание встреч и собраний с помощью EWS в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Создание событий на целый день с помощью EWS в Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Структура DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx)
    
- [Класс Тимезонеинфо](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

