---
title: SortOrder (Конверсатионнодесортордер)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: Элемент SortOrder указывает порядок сортировки, используемый для результатов запроса GetConversationItems.
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530967"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (Конверсатионнодесортордер)

Элемент **SortOrder** указывает порядок сортировки, используемый для результатов запроса **GetConversationItems** . 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **конверсатионнодесортордер**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SortOrder** — это порядок, в котором упорядочиваются обсуждения. Текстовое значение **триордерасцендинг** указывает, что беседы упорядочиваются в соответствии с деревом бесед в возрастающем порядке. Текстовое значение **триордердесцендинг** указывает, что беседы упорядочиваются по дереву бесед в порядке убывания. Текстовое значение **датеордерасцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в возрастающем порядке. Текстовое значение **датеордердесцендинг** указывает, что беседы упорядочиваются в соответствии с датой беседы в убывающем порядке. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> ||
   

