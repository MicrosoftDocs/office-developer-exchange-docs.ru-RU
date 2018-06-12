---
title: BusinessPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: Элемент BusinessPhoneNumbers указывает массив business номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 692c38a00241da9f753c431612f4a8fcf26cc7ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761627"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="9ca38-103">BusinessPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="9ca38-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="9ca38-104">Элемент **BusinessPhoneNumbers** указывает массив business номера телефонов и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ca38-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="9ca38-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9ca38-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ca38-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9ca38-106">Attributes and elements</span></span>

<span data-ttu-id="9ca38-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9ca38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ca38-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9ca38-108">Attributes</span></span>

<span data-ttu-id="9ca38-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9ca38-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ca38-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9ca38-110">Child elements</span></span>

|<span data-ttu-id="9ca38-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9ca38-111">**Element**</span></span>|<span data-ttu-id="9ca38-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ca38-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ca38-113">Значение (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="9ca38-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="9ca38-114">Указывает номер и введите сведения о номерах телефонов и связанный с набором атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9ca38-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="9ca38-115">Атрибуты (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="9ca38-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="9ca38-116">Указывает массив атрибуты для его связанное **значение** элемента.</span><span class="sxs-lookup"><span data-stu-id="9ca38-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ca38-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9ca38-117">Parent elements</span></span>

|<span data-ttu-id="9ca38-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9ca38-118">**Element**</span></span>|<span data-ttu-id="9ca38-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9ca38-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ca38-120">Пользователь</span><span class="sxs-lookup"><span data-stu-id="9ca38-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9ca38-121">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="9ca38-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ca38-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="9ca38-122">Remarks</span></span>

<span data-ttu-id="9ca38-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9ca38-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9ca38-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ca38-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ca38-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9ca38-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ca38-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9ca38-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ca38-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9ca38-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9ca38-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="9ca38-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="9ca38-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9ca38-129">Validation File</span></span>  <br/> |<span data-ttu-id="9ca38-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ca38-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ca38-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9ca38-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9ca38-132">См. также</span><span class="sxs-lookup"><span data-stu-id="9ca38-132">See also</span></span>



- [<span data-ttu-id="9ca38-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9ca38-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
