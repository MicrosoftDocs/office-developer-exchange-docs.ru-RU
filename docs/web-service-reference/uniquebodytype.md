---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: Элемент UniqueBodyType указывает, возвращается ли уникальный текст в формате HTML или текст.
ms.openlocfilehash: c6eb4ec4e39a0c5355775a635db4c63efc666820
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840284"
---
# <a name="uniquebodytype"></a><span data-ttu-id="9591c-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="9591c-103">UniqueBodyType</span></span>

<span data-ttu-id="9591c-104">Элемент **UniqueBodyType** указывает, возвращается ли уникальный текст в формате HTML или текст.</span><span class="sxs-lookup"><span data-stu-id="9591c-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="9591c-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="9591c-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9591c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9591c-106">Attributes and elements</span></span>

<span data-ttu-id="9591c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9591c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9591c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9591c-108">Attributes</span></span>

<span data-ttu-id="9591c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9591c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9591c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9591c-110">Child elements</span></span>

<span data-ttu-id="9591c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9591c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9591c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9591c-112">Parent elements</span></span>

[<span data-ttu-id="9591c-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9591c-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="9591c-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9591c-114">Text value</span></span>

<span data-ttu-id="9591c-115">Текстовое значение элемента **UniqueBodyType** указывает, что формат уникальный body, возвращается в.</span><span class="sxs-lookup"><span data-stu-id="9591c-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="9591c-116">В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="9591c-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="9591c-117">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9591c-117">**Value**</span></span>|<span data-ttu-id="9591c-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9591c-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9591c-119">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="9591c-119">Best</span></span>  <br/> |<span data-ttu-id="9591c-120">В ответе будут возвращены содержательности доступное содержимое основного текста.</span><span class="sxs-lookup"><span data-stu-id="9591c-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="9591c-121">Это полезно, если не известно, является ли содержимое текста или HTML.</span><span class="sxs-lookup"><span data-stu-id="9591c-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="9591c-122">Возвращаемое значение body будет текст основному сохраненных обычного текста.</span><span class="sxs-lookup"><span data-stu-id="9591c-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="9591c-123">В противном случае ответ вернет HTML Если сохраненные текст в формате HTML или RTF.</span><span class="sxs-lookup"><span data-stu-id="9591c-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="9591c-124">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9591c-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="9591c-125">HTML</span><span class="sxs-lookup"><span data-stu-id="9591c-125">HTML</span></span>  <br/> |<span data-ttu-id="9591c-126">В ответе возвращается уникальное body как HTML.</span><span class="sxs-lookup"><span data-stu-id="9591c-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="9591c-127">Text</span><span class="sxs-lookup"><span data-stu-id="9591c-127">Text</span></span>  <br/> |<span data-ttu-id="9591c-128">В ответе возвращается уникальное body как обычный текст.</span><span class="sxs-lookup"><span data-stu-id="9591c-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9591c-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="9591c-129">Remarks</span></span>

<span data-ttu-id="9591c-130">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9591c-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="9591c-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9591c-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9591c-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9591c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9591c-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9591c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9591c-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9591c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9591c-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9591c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="9591c-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9591c-136">Validation File</span></span>  <br/> |<span data-ttu-id="9591c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9591c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9591c-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9591c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9591c-139">True</span><span class="sxs-lookup"><span data-stu-id="9591c-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9591c-140">См. также</span><span class="sxs-lookup"><span data-stu-id="9591c-140">See also</span></span>



[<span data-ttu-id="9591c-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9591c-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="9591c-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9591c-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
