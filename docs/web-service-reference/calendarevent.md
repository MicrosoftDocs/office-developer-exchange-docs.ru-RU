---
title: календаревент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: Элемент Календаревент представляет уникальное вхождение элемента календаря.
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459078"
---
# <a name="calendarevent"></a>календаревент

Элемент **календаревент** представляет уникальное вхождение элемента календаря. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
[календаревентаррай](calendareventarray.md)
  
[календаревент](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 **календаревент**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Представляет начало события календаря. Это обязательный дочерний элемент.  <br/> |
|[EndTime](endtime.md) <br/> |Представляет конец события календаря. Это обязательный дочерний элемент.  <br/> |
|[буситипе](busytype.md) <br/> |Представляет состояние занятости, заданное для события календаря. Это обязательный дочерний элемент.  <br/> |
|[календаревентдетаилс](calendareventdetails.md) <br/> |Предоставляет дополнительные сведения о событии календаря. Это необязательный дочерний элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаревентаррай](calendareventarray.md) <br/> |Содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.  <br/> Ниже приведено выражение XPath 2,0 для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>Примечания

Время встреч и собраний возвращается в часовом поясе клиента. Все дочерние элементы перечислены в той последовательности, в которой они выполняются. Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.
  
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

