---
title: GetOrganizationRelationshipSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: Элемент GetOrganizationRelationshipSettingsRequest представляет параметры звонка на операции GetOrganizationRelationshipSettings операции (SOAP). Элемент GetOrganizationRelationshipSettingsRequest — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 451506d53212ddca416f5b797624688f511988d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762863"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="6764d-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6764d-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="6764d-106">Элемент **GetOrganizationRelationshipSettingsRequest** представляет параметры звонка на операции [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="6764d-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="6764d-107">Элемент **GetOrganizationRelationshipSettingsRequest** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6764d-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="6764d-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="6764d-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="6764d-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="6764d-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6764d-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6764d-110">Attributes and elements</span></span>

<span data-ttu-id="6764d-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6764d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6764d-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6764d-112">Attributes</span></span>

<span data-ttu-id="6764d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6764d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6764d-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6764d-114">Child elements</span></span>

|<span data-ttu-id="6764d-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6764d-115">**Element**</span></span>|<span data-ttu-id="6764d-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6764d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6764d-117">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6764d-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="6764d-118">Представляет коллекцию идентификаторов домена.</span><span class="sxs-lookup"><span data-stu-id="6764d-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="6764d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6764d-119">Parent elements</span></span>

<span data-ttu-id="6764d-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="6764d-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6764d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6764d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6764d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6764d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6764d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6764d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6764d-124">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="6764d-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6764d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6764d-125">Validation File</span></span>  <br/> |<span data-ttu-id="6764d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6764d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6764d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6764d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6764d-128">True</span><span class="sxs-lookup"><span data-stu-id="6764d-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6764d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="6764d-129">See also</span></span>



[<span data-ttu-id="6764d-130">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6764d-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

