---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: Элемент ItemAttachment представляет собой элемент Exchange, подключенный к другой элемент Exchange.
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834137"
---
# <a name="itemattachment"></a>ItemAttachment

Элемент **ItemAttachment** представляет собой элемент Exchange, подключенный к другой элемент Exchange. 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

 **ItemAttachmentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатора вложения AttachmentId](attachmentid.md) <br/> |Идентифицирует вложение.  <br/> |
|[Имя (AttachmentType)](name-attachmenttype.md) <br/> |Представляет имя вложения.  <br/> |
|[ContentType](contenttype.md) <br/> |Описывает тип Multipurpose Internet Mail Extensions (MIME) для содержимого вложения.  <br/> |
|[ContentId](contentid.md) <br/> |Представляет идентификатор содержимого вложения. [ContentId](contentid.md) может быть присвоено любое строковое значение. Приложения могут использовать для реализации идентификации механизмы [ContentId](contentid.md) .  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Содержит универсальный код ресурса (URI), соответствующий расположение содержимого вложения.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах файла вложения.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Представляет после последнего изменения вложения.  <br/> |
|[IsInline](isinline.md) <br/> |Представляет ли вложение встроенным в элемент.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный вложение элемента Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет вложения сообщения электронной почты Exchange.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет вложение элемента календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет вложение элемента контакта Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет вложение задач Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы и/или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
