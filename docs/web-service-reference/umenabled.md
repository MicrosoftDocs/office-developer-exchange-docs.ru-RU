---
title: UmEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: Элемент UmEnabled указывает, включена ли единой системы обмена сообщениями для учетной записи.
ms.openlocfilehash: 8324e02136adc6704bc0badb77131e9671ee569f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840257"
---
# <a name="umenabled"></a><span data-ttu-id="2bd4e-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="2bd4e-103">UmEnabled</span></span>

<span data-ttu-id="2bd4e-104">Элемент **UmEnabled** указывает, включена ли единой системы обмена сообщениями для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="2bd4e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2bd4e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bd4e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2bd4e-106">Attributes and elements</span></span>

<span data-ttu-id="2bd4e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bd4e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2bd4e-108">Attributes</span></span>

<span data-ttu-id="2bd4e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bd4e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2bd4e-110">Child elements</span></span>

<span data-ttu-id="2bd4e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2bd4e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2bd4e-112">Parent elements</span></span>

|<span data-ttu-id="2bd4e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2bd4e-113">**Element**</span></span>|<span data-ttu-id="2bd4e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2bd4e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bd4e-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="2bd4e-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="2bd4e-116">Содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2bd4e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2bd4e-117">Text value</span></span>

<span data-ttu-id="2bd4e-118">Текстовое значение элемента **UmEnabled** имеет **значение true** , если единой системы обмена сообщениями для учетной записи; в противном случае — значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2bd4e-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="2bd4e-119">Remarks</span></span>

<span data-ttu-id="2bd4e-120">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-120">This element is required.</span></span>
  
<span data-ttu-id="2bd4e-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2bd4e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bd4e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2bd4e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bd4e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2bd4e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2bd4e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2bd4e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2bd4e-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2bd4e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2bd4e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2bd4e-126">Validation File</span></span>  <br/> |<span data-ttu-id="2bd4e-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2bd4e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2bd4e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2bd4e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bd4e-129">False</span><span class="sxs-lookup"><span data-stu-id="2bd4e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bd4e-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2bd4e-130">See also</span></span>



- [<span data-ttu-id="2bd4e-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2bd4e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
