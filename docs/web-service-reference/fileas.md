---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: Элемент FileAs — как оформлена списка рассылки или контактов в папке «Контакты».
ms.openlocfilehash: dab9142eebf7691862e7970a7d1e8f5874393b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762539"
---
# <a name="fileas"></a><span data-ttu-id="95746-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="95746-103">FileAs</span></span>

<span data-ttu-id="95746-104">Элемент **FileAs** — как оформлена списка рассылки или контактов в папке «Контакты».</span><span class="sxs-lookup"><span data-stu-id="95746-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="95746-105">**string**</span><span class="sxs-lookup"><span data-stu-id="95746-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95746-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="95746-106">Attributes and elements</span></span>

<span data-ttu-id="95746-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="95746-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95746-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="95746-108">Attributes</span></span>

<span data-ttu-id="95746-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="95746-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95746-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="95746-110">Child elements</span></span>

<span data-ttu-id="95746-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="95746-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95746-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="95746-112">Parent elements</span></span>

|<span data-ttu-id="95746-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95746-113">**Element**</span></span>|<span data-ttu-id="95746-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95746-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95746-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="95746-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="95746-116">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="95746-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="95746-117">Контакт</span><span class="sxs-lookup"><span data-stu-id="95746-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="95746-118">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="95746-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95746-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="95746-119">Text value</span></span>

<span data-ttu-id="95746-120">Текстовое значение, представляющее строку является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="95746-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95746-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="95746-121">Remarks</span></span>

<span data-ttu-id="95746-122">Элемент **FileAs** используется для сортировки контакты и списки рассылки по имени, отличный от полное имя или название компании.</span><span class="sxs-lookup"><span data-stu-id="95746-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="95746-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="95746-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95746-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="95746-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95746-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="95746-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95746-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="95746-126">Schema name</span></span>  <br/> |<span data-ttu-id="95746-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="95746-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="95746-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="95746-128">Validation file</span></span>  <br/> |<span data-ttu-id="95746-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="95746-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95746-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="95746-130">Can be empty</span></span>  <br/> |<span data-ttu-id="95746-131">False</span><span class="sxs-lookup"><span data-stu-id="95746-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95746-132">См. также</span><span class="sxs-lookup"><span data-stu-id="95746-132">See also</span></span>



- [<span data-ttu-id="95746-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="95746-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
