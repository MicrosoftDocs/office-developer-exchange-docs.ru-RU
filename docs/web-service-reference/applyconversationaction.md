---
title: ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: e0ee8f30-529b-4d87-8bc0-b6616e75fb6b
description: Элемент ApplyConversationAction определяет запрос на применение действий к элементам в беседе.
ms.openlocfilehash: 659b3392778bb1a318c3942a0c8e314f12110c12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461690"
---
# <a name="applyconversationaction"></a>ApplyConversationAction

Элемент **ApplyConversationAction** определяет запрос на применение действий к элементам в беседе. 
  
[ApplyConversationAction](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 **аппликонверсатионактионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактионс](conversationactions.md) <br/> |Содержит коллекцию бесед и действий, которые необходимо применить к ним.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

