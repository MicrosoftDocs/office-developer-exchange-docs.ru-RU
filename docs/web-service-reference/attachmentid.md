---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: Элемент AttachmentId определяет вложенный элемент или файл. Этот элемент используется в ответах CreateAttachment.
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459113"
---
# <a name="attachmentid"></a>AttachmentId

Элемент **AttachmentId** определяет вложенный элемент или файл. Этот элемент используется в ответах CreateAttachment. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **аттачментидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Определяет уникальный идентификатор вложения.  <br/> |
|**рутитемид** <br/> |Определяет уникальный идентификатор элемента корневого хранилища, к которому присоединено вложение.  <br/> |
|**рутитемчанжекэй** <br/> |Определяет ключ изменения элемента корневого хранилища, к которому присоединено вложение.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Представляет файл, присоединенный к элементу в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Важно отметить, что при создании вложения изменяется ключ изменения корневого элемента.
  
Элемент [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) используется в запросах DeleteAttachment и GetAttachment. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

