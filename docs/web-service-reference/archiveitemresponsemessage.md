---
title: арчивеитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: Элемент Арчивеитемреспонсемессаже указывает ответное сообщение на запрос ArchiveItem.
ms.openlocfilehash: 24d09d63cab6805194e35031d8590290573de0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463393"
---
# <a name="archiveitemresponsemessage"></a>арчивеитемреспонсемессаже

Элемент **арчивеитемреспонсемессаже** указывает ответное сообщение на запрос **ArchiveItem** . 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 **итеминфореспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|респонсекласс  <br/> |Указывает класс ответа.  <br/> |
   
#### <a name="responseclass"></a>респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|Успешно  <br/> |Указывает на успешное выполнение.  <br/> |
|Предупреждение  <br/> |Указывает на предупреждение.  <br/> |
|Ошибка  <br/> |Указывает на ошибку.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для будущего использования.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет сведения о состоянии запроса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

