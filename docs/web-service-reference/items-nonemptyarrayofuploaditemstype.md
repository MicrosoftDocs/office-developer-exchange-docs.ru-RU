---
title: Элементы (NonEmptyArrayOfUploadItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 402bfa6d-11d7-4547-b8bd-197e9922ab49
description: Элемент элементов содержит массив элементов для передачи в почтовый ящик.
ms.openlocfilehash: ac508b2026c3e0ec730154efeeff0a9669e6eff8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834156"
---
# <a name="items-nonemptyarrayofuploaditemstype"></a><span data-ttu-id="c2cbe-103">Элементы (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="c2cbe-103">Items (NonEmptyArrayOfUploadItemsType)</span></span>

<span data-ttu-id="c2cbe-104">Элемент **элементов** содержит массив элементов для передачи в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-104">The **Items** element contains an array of items to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="c2cbe-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="c2cbe-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="c2cbe-106">Элементы (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="c2cbe-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
```XML
<Items>
   <Item/>
</Items>
```

 <span data-ttu-id="c2cbe-107">**NonEmptyArrayOfUploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="c2cbe-107">**NonEmptyArrayOfUploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2cbe-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c2cbe-108">Attributes and elements</span></span>

<span data-ttu-id="c2cbe-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2cbe-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c2cbe-110">Attributes</span></span>

<span data-ttu-id="c2cbe-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2cbe-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c2cbe-112">Child elements</span></span>

|<span data-ttu-id="c2cbe-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2cbe-113">**Element**</span></span>|<span data-ttu-id="c2cbe-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2cbe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2cbe-115">Элемент (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="c2cbe-115">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="c2cbe-116">Представляет один элемент для передачи в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-116">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2cbe-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c2cbe-117">Parent elements</span></span>

|<span data-ttu-id="c2cbe-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2cbe-118">**Element**</span></span>|<span data-ttu-id="c2cbe-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2cbe-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2cbe-120">UploadItems</span><span class="sxs-lookup"><span data-stu-id="c2cbe-120">UploadItems</span></span>](uploaditems.md) <br/> |<span data-ttu-id="c2cbe-121">Представляет запрос для загрузки элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-121">Represents a request to upload items into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2cbe-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c2cbe-122">Text value</span></span>

<span data-ttu-id="c2cbe-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c2cbe-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2cbe-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="c2cbe-124">Remarks</span></span>

<span data-ttu-id="c2cbe-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c2cbe-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2cbe-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c2cbe-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2cbe-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c2cbe-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2cbe-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c2cbe-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c2cbe-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="c2cbe-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="c2cbe-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c2cbe-130">Validation File</span></span>  <br/> |<span data-ttu-id="c2cbe-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2cbe-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2cbe-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c2cbe-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2cbe-133">False</span><span class="sxs-lookup"><span data-stu-id="c2cbe-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2cbe-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c2cbe-134">See also</span></span>



[<span data-ttu-id="c2cbe-135">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="c2cbe-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="c2cbe-136">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="c2cbe-136">UploadItems operation</span></span>](uploaditems-operation.md)
