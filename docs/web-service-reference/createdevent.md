---
title: CreatedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreatedEvent
api_type:
- schema
ms.assetid: f0e53a53-c352-42a5-8280-cd808b0e961b
description: CreatedEvent элемент представляет событие, в котором создается элемента или папки.
ms.openlocfilehash: f52516090d0789b4dd9fc1ced824786ce000e885
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761864"
---
# <a name="createdevent"></a>CreatedEvent

**CreatedEvent** элемент представляет событие, в котором создается элемента или папки. 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 **BaseObjectChangedEventType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Водяной знак](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика.  <br/> |
|[Метка времени](timestamp.md) <br/> |Представляет отметки времени событии создания элемента или папки почтового ящика.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор созданного папки.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Представляет идентификатор созданного элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, созданной элемента или папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)


[С помощью подписки по запросу](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[Уведомления о событиях в веб-служб Exchange](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
