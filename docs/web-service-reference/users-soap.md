---
title: Пользователи (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: Элемент Users представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры.
ms.openlocfilehash: d7655f0020a315dcb32adbbc58610ca0e630c1fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840440"
---
# <a name="users-soap"></a><span data-ttu-id="ea805-103">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea805-103">Users (SOAP)</span></span>

<span data-ttu-id="ea805-104">Элемент **Users** представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="ea805-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="ea805-105">**пользователи**;</span><span class="sxs-lookup"><span data-stu-id="ea805-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea805-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea805-106">Attributes and elements</span></span>

<span data-ttu-id="ea805-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ea805-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea805-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea805-108">Attributes</span></span>

<span data-ttu-id="ea805-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea805-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea805-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea805-110">Child elements</span></span>

|<span data-ttu-id="ea805-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea805-111">**Element**</span></span>|<span data-ttu-id="ea805-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea805-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea805-113">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea805-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="ea805-114">Представляет адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="ea805-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea805-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea805-115">Parent elements</span></span>

|<span data-ttu-id="ea805-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea805-116">**Element**</span></span>|<span data-ttu-id="ea805-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea805-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea805-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea805-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="ea805-119">Представляет запрос для получения параметров указанного для одного или нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea805-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="ea805-120">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea805-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="ea805-121">Содержит параметры запрошенные конфигурации и к конечным пользователям.</span><span class="sxs-lookup"><span data-stu-id="ea805-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea805-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ea805-122">Text value</span></span>

<span data-ttu-id="ea805-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea805-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea805-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea805-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea805-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea805-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ea805-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea805-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ea805-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="ea805-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ea805-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea805-128">Validation File</span></span>  <br/> |<span data-ttu-id="ea805-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea805-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea805-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea805-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea805-131">True</span><span class="sxs-lookup"><span data-stu-id="ea805-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea805-132">См. также</span><span class="sxs-lookup"><span data-stu-id="ea805-132">See also</span></span>



[<span data-ttu-id="ea805-133">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea805-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

