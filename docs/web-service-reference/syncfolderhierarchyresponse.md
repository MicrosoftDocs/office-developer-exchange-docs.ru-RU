---
title: SyncFolderHierarchyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponse
api_type:
- schema
ms.assetid: 7e6061d2-bbce-4864-a7bb-a6457628cb7c
description: Элемент SyncFolderHierarchyResponse определяет ответ на запрос SyncFolderHierarchy.
ms.openlocfilehash: aee70603b84dfdf5f7f580fd2566f7ebfbbce383
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840124"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="c526b-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c526b-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="c526b-104">Элемент **SyncFolderHierarchyResponse** определяет ответ на запрос SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="c526b-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="c526b-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="c526b-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c526b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c526b-106">Attributes and elements</span></span>

<span data-ttu-id="c526b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c526b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c526b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c526b-108">Attributes</span></span>

<span data-ttu-id="c526b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c526b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c526b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c526b-110">Child elements</span></span>

|<span data-ttu-id="c526b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c526b-111">**Element**</span></span>|<span data-ttu-id="c526b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c526b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c526b-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c526b-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c526b-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="c526b-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c526b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c526b-115">Parent elements</span></span>

<span data-ttu-id="c526b-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="c526b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c526b-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="c526b-117">Remarks</span></span>

<span data-ttu-id="c526b-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c526b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c526b-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c526b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c526b-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c526b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c526b-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c526b-121">Schema name</span></span>  <br/> |<span data-ttu-id="c526b-122">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="c526b-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="c526b-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c526b-123">Validation file</span></span>  <br/> |<span data-ttu-id="c526b-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c526b-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c526b-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c526b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="c526b-126">False</span><span class="sxs-lookup"><span data-stu-id="c526b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c526b-127">См. также</span><span class="sxs-lookup"><span data-stu-id="c526b-127">See also</span></span>



[<span data-ttu-id="c526b-128">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c526b-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="c526b-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c526b-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
