---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: Элемент ExtendedPropertyAttributedValue указывает расширенные свойства для пользователя.
ms.openlocfilehash: 92e4ec7f192ccb36ea68d7862e66cb7b3349819a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762469"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="f341f-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f341f-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="f341f-104">Элемент **ExtendedPropertyAttributedValue** указывает расширенные свойства для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f341f-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="f341f-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="f341f-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f341f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f341f-106">Attributes and elements</span></span>

<span data-ttu-id="f341f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f341f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f341f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f341f-108">Attributes</span></span>

<span data-ttu-id="f341f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f341f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f341f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f341f-110">Child elements</span></span>

|<span data-ttu-id="f341f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f341f-111">**Element**</span></span>|<span data-ttu-id="f341f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f341f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f341f-113">Значение (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="f341f-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="f341f-114">Указывает массив расширенных свойств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f341f-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="f341f-115">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="f341f-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="f341f-116">Указывает массив атрибуты для его связанное **значение** элемента.</span><span class="sxs-lookup"><span data-stu-id="f341f-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f341f-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f341f-117">Parent elements</span></span>

|<span data-ttu-id="f341f-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f341f-118">**Element**</span></span>|<span data-ttu-id="f341f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f341f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f341f-120">Свойство ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="f341f-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="f341f-121">Содержит расширенные свойства, используемые для операций единого хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="f341f-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f341f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="f341f-122">Remarks</span></span>

<span data-ttu-id="f341f-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f341f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f341f-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f341f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f341f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f341f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f341f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f341f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f341f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f341f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f341f-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f341f-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f341f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f341f-129">Validation File</span></span>  <br/> |<span data-ttu-id="f341f-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f341f-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f341f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f341f-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f341f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f341f-132">See also</span></span>



- [<span data-ttu-id="f341f-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f341f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

