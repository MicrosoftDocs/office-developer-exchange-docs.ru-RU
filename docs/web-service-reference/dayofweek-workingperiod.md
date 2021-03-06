---
title: DayOfWeek (Воркингпериод)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: Элемент DayOfWeek содержит список рабочих дней, запланированных для пользователя почтового ящика.
ms.openlocfilehash: 06d4a7d5541b3b71fcbf9be9beb7512d06853283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457447"
---
# <a name="dayofweek-workingperiod"></a>DayOfWeek (Воркингпериод)

Элемент **DayOfWeek** содержит список рабочих дней, запланированных для пользователя почтового ящика. 
  
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)  
- [фрибусиреспонсеаррай](freebusyresponsearray.md)  
- [фрибусиреспонсе](freebusyresponse.md)  
- [фрибусивиев](freebusyview.md)  
- [воркингхаурс](workinghours-ex15websvcsotherref.md)  
- [воркингпериодаррай](workingperiodarray.md) 
- [воркингпериод](workingperiod.md)  
- [DayOfWeek (Воркингпериод)](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

**DaysOfWeek**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[воркингпериод](workingperiod.md) <br/> |Содержит рабочие недели, дни и часы пользователя почтового ящика.<br/><br/>Ниже приведено выражение XPath для этого элемента:<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение возвращается, если у пользователя почтового ящика есть дни, настроенные для представления рабочей недели. Ниже приведены возможные значения для этого элемента.
  
- Воскресеньям    
- Понедельник    
- Вторник    
- Среда    
- Четверг    
- Пятница    
- Суббота 
    
Текстовые значения будут возвращены в указанном порядке.
  
## <a name="remarks"></a>Примечания

Важно отметить, что разница между этим элементом и элементом доступности [DayOfWeek (TimeZone)](dayofweek-timezone.md) — это тип. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)  
- [жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

