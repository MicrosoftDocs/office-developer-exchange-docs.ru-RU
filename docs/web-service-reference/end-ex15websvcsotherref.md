---
title: Конец
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: Элемент End представляет конец длительности.
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456145"
---
# <a name="end"></a>Конец

Элемент **End** представляет конец длительности. 
  
```xml
<End/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[фирстоккурренце](firstoccurrence.md) <br/> |Представляет первое вхождение повторяющегося элемента календаря.  <br/> |
|[ластоккурренце](lastoccurrence.md) <br/> |Представляет последнее вхождение повторяющегося элемента календаря.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[Экземпляр](occurrence.md) <br/> |Представляет один измененный экземпляр повторяющегося элемента календаря.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет конец длительности.
  
## <a name="remarks"></a>Примечания

Для операции UpdateItem можно задать время [начала](start.md) и **окончания** для элемента хранилища Exchange. В запросе UpdateItem вы можете задать время [начала](start.md) , не устанавливая и время **окончания** . Это может привести к ошибке, если время [начала](start.md) позже времени **окончания** . Имейте в виду, что клиентские приложения должны выполнить корректировку до времени **окончания** при изменении времени [начала](start.md) , чтобы сохранить длительность. 
  
 **Note (Примечание** ) Сведения о смещении часового пояса теряются, если даты [начала](start.md) и **окончания** повторяющегося элемента шаблона не имеют даты, равной первому появлению еженедельного расписания повторения. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[виклирекурренце](weeklyrecurrence.md)
  
 **End**


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

