---
title: воркингхаурс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: Элемент Воркингхаурс представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.
ms.openlocfilehash: 9cb21e72f7024b96b4b5f252a8a3b85bb704e67c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468343"
---
# <a name="workinghours"></a>воркингхаурс

Элемент **воркингхаурс** представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
[воркингхаурс](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 **воркингхаурс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Часовой пояс (доступность)](timezone-availability.md) <br/> |Содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе со стандартного времени на летнее время. Этот элемент является обязательным, если используется элемент **воркингхаурс** .  <br/> |
|[воркингпериодаррай](workingperiodarray.md) <br/> |Содержит сведения о рабочем периоде для пользователя почтового ящика. Этот элемент является обязательным, если используется элемент **воркингхаурс** .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусивиев](freebusyview.md) <br/> |Содержит сведения о доступности для определенного пользователя.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a>Примечания

Все дочерние элементы перечислены в той последовательности, в которой они выполняются. Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

