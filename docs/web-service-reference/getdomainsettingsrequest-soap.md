---
title: Жетдомаинсеттингсрекуест (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: Элемент Жетдомаинсеттингсрекуест представляет запрос операции Жетдомаинсеттингс (SOAP).
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460962"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="86019-103">Жетдомаинсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86019-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="86019-104">Элемент **жетдомаинсеттингсрекуест** представляет запрос операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="86019-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="86019-105">**жетдомаинсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="86019-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86019-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="86019-106">Attributes and elements</span></span>

<span data-ttu-id="86019-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="86019-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86019-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="86019-108">Attributes</span></span>

<span data-ttu-id="86019-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86019-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86019-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="86019-110">Child elements</span></span>

|<span data-ttu-id="86019-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="86019-111">**Element**</span></span>|<span data-ttu-id="86019-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="86019-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86019-113">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86019-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="86019-114">Представляет коллекцию идентификаторов доменов.</span><span class="sxs-lookup"><span data-stu-id="86019-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="86019-115">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86019-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="86019-116">Содержит имена запрошенных параметров конфигурации домена.</span><span class="sxs-lookup"><span data-stu-id="86019-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="86019-117">Рекуестедверсион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86019-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="86019-118">Указывает версию сервера, который будет использоваться поставщиком.</span><span class="sxs-lookup"><span data-stu-id="86019-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86019-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="86019-119">Parent elements</span></span>

<span data-ttu-id="86019-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86019-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="86019-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="86019-121">Text value</span></span>

<span data-ttu-id="86019-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86019-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86019-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="86019-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86019-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="86019-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="86019-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="86019-125">Schema Name</span></span>  <br/> |<span data-ttu-id="86019-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="86019-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="86019-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="86019-127">Validation File</span></span>  <br/> |<span data-ttu-id="86019-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="86019-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86019-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="86019-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="86019-130">True</span><span class="sxs-lookup"><span data-stu-id="86019-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86019-131">См. также</span><span class="sxs-lookup"><span data-stu-id="86019-131">See also</span></span>



[<span data-ttu-id="86019-132">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86019-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

