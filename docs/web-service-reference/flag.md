---
title: Отметка
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Элемент флаг указывает флаг для элемента почтового ящика.
ms.openlocfilehash: f30f435e8f064d7165ae52de737bbd75b0546206
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762607"
---
# <a name="flag"></a>Отметка

Элемент **флаг** указывает флаг для элемента почтового ящика. 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **FlagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |Содержит объединенные флаг состояния для элементов в текущей папке.  <br/> |
|[Дата начала](startdate.md) <br/> |Представляет дату начала элемента.  <br/> |
|[DueDate](duedate.md) <br/> |Представляет дату, когда срок выполнения элемента.  <br/> |
|[CompleteDate](completedate.md) <br/> |Представляет дату, на котором был выполнен элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Содержит одно действие должен применяться к разговора.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
