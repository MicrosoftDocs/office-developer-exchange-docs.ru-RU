---
title: WithinSizeRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: Элемент WithinSizeRange указывает минимальный и максимальный размеры, которые должны быть входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 7711db9ca68f972f080c98197e30c7710620119a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840521"
---
# <a name="withinsizerange"></a><span data-ttu-id="5cbb1-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="5cbb1-103">WithinSizeRange</span></span>

<span data-ttu-id="5cbb1-104">Элемент **WithinSizeRange** указывает минимальный и максимальный размеры, которые должны быть входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="5cbb1-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="5cbb1-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cbb1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5cbb1-106">Attributes and elements</span></span>

<span data-ttu-id="5cbb1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cbb1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5cbb1-108">Attributes</span></span>

<span data-ttu-id="5cbb1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cbb1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5cbb1-110">Child elements</span></span>

|<span data-ttu-id="5cbb1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5cbb1-111">**Element**</span></span>|<span data-ttu-id="5cbb1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5cbb1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cbb1-113">Минимальный размер</span><span class="sxs-lookup"><span data-stu-id="5cbb1-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="5cbb1-114">Указывает минимальный размер, сообщения должны быть в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="5cbb1-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="5cbb1-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="5cbb1-116">Указывает максимальный размер, сообщения должны быть в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cbb1-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5cbb1-117">Parent elements</span></span>

|<span data-ttu-id="5cbb1-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5cbb1-118">**Element**</span></span>|<span data-ttu-id="5cbb1-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5cbb1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cbb1-120">Условия</span><span class="sxs-lookup"><span data-stu-id="5cbb1-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5cbb1-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5cbb1-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="5cbb1-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5cbb1-123">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="5cbb1-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cbb1-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5cbb1-124">Text value</span></span>

<span data-ttu-id="5cbb1-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5cbb1-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="5cbb1-126">Remarks</span></span>

<span data-ttu-id="5cbb1-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cbb1-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cbb1-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5cbb1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cbb1-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5cbb1-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5cbb1-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5cbb1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5cbb1-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5cbb1-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5cbb1-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5cbb1-132">Validation File</span></span>  <br/> |<span data-ttu-id="5cbb1-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5cbb1-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cbb1-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5cbb1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cbb1-135">True</span><span class="sxs-lookup"><span data-stu-id="5cbb1-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cbb1-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5cbb1-136">See also</span></span>



- [<span data-ttu-id="5cbb1-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5cbb1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

