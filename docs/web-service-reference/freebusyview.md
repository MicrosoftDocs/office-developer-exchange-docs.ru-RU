---
title: фрибусивиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: Элемент Фрибусивиев содержит сведения о доступности для определенного пользователя.
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456103"
---
# <a name="freebusyview"></a>фрибусивиев

Элемент **фрибусивиев** содержит сведения о доступности для определенного пользователя. 
  
[жетусераваилабилитиреспонсе](getuseravailabilityresponse.md)
  
[фрибусиреспонсеаррай](freebusyresponsearray.md)
  
[фрибусиреспонсе](freebusyresponse.md)
  
[фрибусивиев](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 **фрибусивиев**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусивиевтипе](freebusyviewtype.md) <br/> |Представляет тип запрошенных сведений о доступности, возвращаемых в ответе.  <br/> |
|[мержедфрибуси](mergedfreebusy.md) <br/> |Содержит Объединенный поток данных о занятости.  <br/> |
|[календаревентаррай](calendareventarray.md) <br/> |Содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.  <br/> |
|[воркингхаурс](workinghours-ex15websvcsotherref.md) <br/> |Представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фрибусиреспонсе](freebusyresponse.md) <br/> |Содержит сведения о доступности для одного пользователя почтового ящика.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
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

