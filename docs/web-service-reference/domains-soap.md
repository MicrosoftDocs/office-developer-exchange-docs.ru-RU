---
title: Домены (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Элемент домены представляет коллекцию домена, который возвращается в операции GetDomainSettings (SOAP), доменов, в ходе операции GetFederationInformation (SOAP) федеративных организации или домены с связь организации как возвращенные операцией GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 7a21a3a09516de2d1c38021ca3ccd2161d9cdd1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762214"
---
# <a name="domains-soap"></a><span data-ttu-id="22fa5-103">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-103">Domains (SOAP)</span></span>

<span data-ttu-id="22fa5-104">Элемент **домены** представляет коллекцию домена, который возвращается в [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), доменов, в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)федеративных организации или домены с связь организации, возвращенные операцией [GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="22fa5-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="22fa5-105">**Домены**</span><span class="sxs-lookup"><span data-stu-id="22fa5-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22fa5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22fa5-106">Attributes and elements</span></span>

<span data-ttu-id="22fa5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="22fa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22fa5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22fa5-108">Attributes</span></span>

<span data-ttu-id="22fa5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="22fa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22fa5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22fa5-110">Child elements</span></span>

|<span data-ttu-id="22fa5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22fa5-111">**Element**</span></span>|<span data-ttu-id="22fa5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22fa5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22fa5-113">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="22fa5-114">Представляет один домен.</span><span class="sxs-lookup"><span data-stu-id="22fa5-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22fa5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22fa5-115">Parent elements</span></span>

|<span data-ttu-id="22fa5-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22fa5-116">**Element**</span></span>|<span data-ttu-id="22fa5-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22fa5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22fa5-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="22fa5-119">Представляет запрос [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="22fa5-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="22fa5-120">Ответ (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="22fa5-121">Содержит сведения, ответа [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="22fa5-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="22fa5-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="22fa5-123">Представляет запрос [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="22fa5-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22fa5-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="22fa5-124">Text value</span></span>

<span data-ttu-id="22fa5-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="22fa5-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22fa5-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22fa5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22fa5-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22fa5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="22fa5-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22fa5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="22fa5-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="22fa5-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="22fa5-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22fa5-130">Validation File</span></span>  <br/> |<span data-ttu-id="22fa5-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22fa5-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22fa5-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22fa5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="22fa5-133">True</span><span class="sxs-lookup"><span data-stu-id="22fa5-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22fa5-134">См. также</span><span class="sxs-lookup"><span data-stu-id="22fa5-134">See also</span></span>

- [<span data-ttu-id="22fa5-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="22fa5-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22fa5-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)
