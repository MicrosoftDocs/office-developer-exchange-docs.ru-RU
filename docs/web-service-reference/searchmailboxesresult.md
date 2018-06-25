---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: Элемент SearchMailboxesResult содержит результат запроса SearchMailboxes.
ms.openlocfilehash: 93e5837216ef8942b77ac2a91f5ef5f0ad001756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835300"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

Элемент **SearchMailboxesResult** содержит результат запроса **SearchMailboxes** . 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 **SearchMailboxesResultType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [размер (длинный)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [элементов () ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [уточнений](refiners.md) | [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>Родительские элементы

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |Нет  <br/> |
   

