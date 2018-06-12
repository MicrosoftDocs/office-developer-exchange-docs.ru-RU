---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: Элемент RequestedSettings содержит имена параметров запрошенные конфигурации.
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835136"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="975fa-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="975fa-104">Элемент **RequestedSettings** содержит имена параметров запрошенные конфигурации.</span><span class="sxs-lookup"><span data-stu-id="975fa-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="975fa-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="975fa-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="975fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="975fa-106">Attributes and elements</span></span>

<span data-ttu-id="975fa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="975fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="975fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="975fa-108">Attributes</span></span>

<span data-ttu-id="975fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="975fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="975fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="975fa-110">Child elements</span></span>

|<span data-ttu-id="975fa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="975fa-111">**Element**</span></span>|<span data-ttu-id="975fa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="975fa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="975fa-113">Параметр (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="975fa-114">Представляет параметр конфигурации должно быть возвращено.</span><span class="sxs-lookup"><span data-stu-id="975fa-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="975fa-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="975fa-115">Parent elements</span></span>

|<span data-ttu-id="975fa-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="975fa-116">**Element**</span></span>|<span data-ttu-id="975fa-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="975fa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="975fa-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="975fa-119">Представляет запрос для получения параметров указанного для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="975fa-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="975fa-120">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="975fa-121">Содержит параметры запрошенные конфигурации и к конечным пользователям.</span><span class="sxs-lookup"><span data-stu-id="975fa-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="975fa-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="975fa-123">Представляет запрос [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="975fa-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="975fa-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="975fa-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="975fa-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="975fa-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="975fa-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="975fa-126">Schema Name</span></span>  <br/> |<span data-ttu-id="975fa-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="975fa-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="975fa-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="975fa-128">Validation File</span></span>  <br/> |<span data-ttu-id="975fa-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="975fa-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="975fa-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="975fa-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="975fa-131">True</span><span class="sxs-lookup"><span data-stu-id="975fa-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="975fa-132">См. также</span><span class="sxs-lookup"><span data-stu-id="975fa-132">See also</span></span>



[<span data-ttu-id="975fa-133">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="975fa-134">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="975fa-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
