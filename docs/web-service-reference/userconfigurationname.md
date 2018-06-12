---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: Элемент UserConfigurationName представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.
ms.openlocfilehash: 40580343e92493c3d39b090371708269ec3274b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840412"
---
# <a name="userconfigurationname"></a><span data-ttu-id="0f002-104">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="0f002-104">UserConfigurationName</span></span>

<span data-ttu-id="0f002-105">Элемент **UserConfigurationName** представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="0f002-106">Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

 <span data-ttu-id="0f002-107">**UserConfigurationNameType**</span><span class="sxs-lookup"><span data-stu-id="0f002-107">**UserConfigurationNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f002-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0f002-108">Attributes and elements</span></span>

<span data-ttu-id="0f002-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0f002-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f002-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0f002-110">Attributes</span></span>

|<span data-ttu-id="0f002-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0f002-111">**Attribute**</span></span>|<span data-ttu-id="0f002-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f002-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0f002-113">**Name**</span><span class="sxs-lookup"><span data-stu-id="0f002-113">**Name**</span></span> <br/> |<span data-ttu-id="0f002-114">Содержит строковое значение, представляющее имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="0f002-115">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="0f002-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0f002-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0f002-116">Child elements</span></span>

|<span data-ttu-id="0f002-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f002-117">**Element**</span></span>|<span data-ttu-id="0f002-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f002-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f002-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="0f002-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0f002-120">Представляет идентификатор папки папку, содержащую объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="0f002-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0f002-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0f002-122">Представляет имя различающегося папки папку, содержащую объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f002-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0f002-123">Parent elements</span></span>

|<span data-ttu-id="0f002-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f002-124">**Element**</span></span>|<span data-ttu-id="0f002-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f002-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f002-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f002-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="0f002-127">Представляет запрос на удаление объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="0f002-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f002-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="0f002-129">Представляет запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="0f002-130">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f002-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="0f002-131">Определяет объект конфигурации одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f002-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f002-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0f002-132">Text value</span></span>

<span data-ttu-id="0f002-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f002-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f002-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="0f002-134">Remarks</span></span>

<span data-ttu-id="0f002-135">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f002-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f002-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0f002-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f002-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0f002-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f002-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0f002-138">Schema Name</span></span>  <br/> |<span data-ttu-id="0f002-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0f002-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f002-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0f002-140">Validation File</span></span>  <br/> |<span data-ttu-id="0f002-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f002-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f002-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0f002-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f002-143">False</span><span class="sxs-lookup"><span data-stu-id="0f002-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f002-144">См. также</span><span class="sxs-lookup"><span data-stu-id="0f002-144">See also</span></span>



- [<span data-ttu-id="0f002-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0f002-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
