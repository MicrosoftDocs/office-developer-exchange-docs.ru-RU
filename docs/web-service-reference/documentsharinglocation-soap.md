---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: Элемент DocumentSharingLocation содержит местоположение и сведения о метаданных для общего доступа к расположение документа.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762198"
---
# <a name="documentsharinglocation-soap"></a><span data-ttu-id="a2edb-103">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-103">DocumentSharingLocation (SOAP)</span></span>

<span data-ttu-id="a2edb-104">Элемент **DocumentSharingLocation** содержит местоположение и сведения о метаданных для общего доступа к расположение документа.</span><span class="sxs-lookup"><span data-stu-id="a2edb-104">The **DocumentSharingLocation** element contains location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 <span data-ttu-id="a2edb-105">**DocumentSharingLocation**</span><span class="sxs-lookup"><span data-stu-id="a2edb-105">**DocumentSharingLocation**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2edb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2edb-106">Attributes and elements</span></span>

<span data-ttu-id="a2edb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2edb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2edb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2edb-108">Attributes</span></span>

<span data-ttu-id="a2edb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2edb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2edb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2edb-110">Child elements</span></span>

|<span data-ttu-id="a2edb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2edb-111">**Element**</span></span>|<span data-ttu-id="a2edb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2edb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2edb-113">ServiceUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-113">ServiceUrl (SOAP)</span></span>](serviceurl-soap.md) <br/> |<span data-ttu-id="a2edb-114">Представляет URL-адрес документа, общий доступ к веб-службе.</span><span class="sxs-lookup"><span data-stu-id="a2edb-114">Represents the URL of the document sharing web service.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-115">LocationUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-115">LocationUrl (SOAP)</span></span>](locationurl-soap.md) <br/> |<span data-ttu-id="a2edb-116">Представляет URL-адрес документа, общий доступ к расположения.</span><span class="sxs-lookup"><span data-stu-id="a2edb-116">Represents the URL of the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-117">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-117">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="a2edb-118">Представляет имя документа, общий доступ к папка, которая используется в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="a2edb-118">Represents the name of the document sharing location to use in the UI.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-119">SupportedFileExtensions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-119">SupportedFileExtensions (SOAP)</span></span>](supportedfileextensions-soap.md) <br/> |<span data-ttu-id="a2edb-120">Представляет расширений файлов, которые могут храниться в документе общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="a2edb-120">Represents the file extensions that can be stored in the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-121">ExternalAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-121">ExternalAccessAllowed (SOAP)</span></span>](externalaccessallowed-soap.md) <br/> |<span data-ttu-id="a2edb-122">Указывает, является ли документ, общий доступ к расположение доступны за пределами подключений.</span><span class="sxs-lookup"><span data-stu-id="a2edb-122">Indicates whether the document sharing location is available to outside connections.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-123">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-123">AnonymousAccessAllowed (SOAP)</span></span>](anonymousaccessallowed-soap.md) <br/> |<span data-ttu-id="a2edb-124">Указывает, требуется ли доступ к месту общего доступа пользователя с разрешением.</span><span class="sxs-lookup"><span data-stu-id="a2edb-124">Indicates whether access to the sharing location requires an authenticated user.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-125">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-125">CanModifyPermissions (SOAP)</span></span>](canmodifypermissions-soap.md) <br/> |<span data-ttu-id="a2edb-126">Указывает, является ли пользователь может изменить разрешения на доступ к документу общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="a2edb-126">Indicates whether the user can modify access permissions to the document sharing location.</span></span>  <br/> |
|[<span data-ttu-id="a2edb-127">IsDefault (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-127">IsDefault (SOAP)</span></span>](isdefault-soap.md) <br/> |<span data-ttu-id="a2edb-128">Указывает, является ли документ, общий доступ к расположение общего доступа расположение по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2edb-128">Indicates whether the document sharing location is the user's default sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2edb-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2edb-129">Parent elements</span></span>

|<span data-ttu-id="a2edb-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2edb-130">**Element**</span></span>|<span data-ttu-id="a2edb-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2edb-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2edb-132">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-132">DocumentSharingLocations (SOAP)</span></span>](documentsharinglocations-soap.md) <br/> |<span data-ttu-id="a2edb-133">Содержит список документов, совместное использование расположения и метаданных.</span><span class="sxs-lookup"><span data-stu-id="a2edb-133">Contains a list of document sharing locations and metadata.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2edb-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a2edb-134">Text value</span></span>

<span data-ttu-id="a2edb-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2edb-135">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2edb-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2edb-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2edb-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2edb-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a2edb-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2edb-138">Schema Name</span></span>  <br/> |<span data-ttu-id="a2edb-139">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a2edb-139">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a2edb-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2edb-140">Validation File</span></span>  <br/> |<span data-ttu-id="a2edb-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2edb-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2edb-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2edb-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2edb-143">True</span><span class="sxs-lookup"><span data-stu-id="a2edb-143">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2edb-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a2edb-144">See also</span></span>

- [<span data-ttu-id="a2edb-145">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2edb-145">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="a2edb-146">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="a2edb-146">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="a2edb-147">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a2edb-147">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
