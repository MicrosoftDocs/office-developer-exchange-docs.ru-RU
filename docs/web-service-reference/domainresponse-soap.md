---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: Элемент DomainResponse содержит запрошенные параметры для конкретного домена.
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762207"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="33f88-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="33f88-104">Элемент **DomainResponse** содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="33f88-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="33f88-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="33f88-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33f88-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33f88-106">Attributes and elements</span></span>

<span data-ttu-id="33f88-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="33f88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33f88-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33f88-108">Attributes</span></span>

<span data-ttu-id="33f88-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="33f88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33f88-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33f88-110">Child elements</span></span>

|<span data-ttu-id="33f88-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33f88-111">**Element**</span></span>|<span data-ttu-id="33f88-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33f88-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33f88-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="33f88-114">Содержит сведения об ошибке для параметров, которые не будут получены.</span><span class="sxs-lookup"><span data-stu-id="33f88-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="33f88-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="33f88-116">Представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="33f88-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="33f88-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="33f88-118">Определяет целевой в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="33f88-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="33f88-119">Целевой объект может быть URL-адрес или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="33f88-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="33f88-120">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="33f88-121">Задает код ошибки, связанный с данным запросом.</span><span class="sxs-lookup"><span data-stu-id="33f88-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="33f88-122">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="33f88-123">Задает сообщение об ошибке, связанный с данным запросом.</span><span class="sxs-lookup"><span data-stu-id="33f88-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33f88-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33f88-124">Parent elements</span></span>

|<span data-ttu-id="33f88-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33f88-125">**Element**</span></span>|<span data-ttu-id="33f88-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33f88-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33f88-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="33f88-128">Содержит массив элементов **DomainResponse** .</span><span class="sxs-lookup"><span data-stu-id="33f88-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="33f88-129">Каждый элемент **DomainResponse** содержит запрошенные параметры для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="33f88-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="33f88-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="33f88-131">Содержит ответы для каждого домена.</span><span class="sxs-lookup"><span data-stu-id="33f88-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33f88-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33f88-132">Text value</span></span>

<span data-ttu-id="33f88-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="33f88-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33f88-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33f88-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33f88-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33f88-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="33f88-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33f88-136">Schema Name</span></span>  <br/> |<span data-ttu-id="33f88-137">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="33f88-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="33f88-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33f88-138">Validation File</span></span>  <br/> |<span data-ttu-id="33f88-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33f88-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33f88-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33f88-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="33f88-141">True</span><span class="sxs-lookup"><span data-stu-id="33f88-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33f88-142">См. также</span><span class="sxs-lookup"><span data-stu-id="33f88-142">See also</span></span>

- [<span data-ttu-id="33f88-143">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33f88-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
