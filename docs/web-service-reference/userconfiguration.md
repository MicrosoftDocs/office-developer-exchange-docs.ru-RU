---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: Элемент UserConfiguration определяет объект конфигурации одного пользователя.
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840413"
---
# <a name="userconfiguration"></a><span data-ttu-id="55011-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55011-103">UserConfiguration</span></span>

<span data-ttu-id="55011-104">Элемент **UserConfiguration** определяет объект конфигурации одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="55011-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="55011-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55011-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55011-106">Attributes and elements</span></span>

<span data-ttu-id="55011-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="55011-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55011-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55011-108">Attributes</span></span>

<span data-ttu-id="55011-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="55011-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55011-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55011-110">Child elements</span></span>

|<span data-ttu-id="55011-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55011-111">**Element**</span></span>|<span data-ttu-id="55011-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55011-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55011-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="55011-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="55011-114">Представляет имя объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="55011-115">Этот элемент должен использоваться при создании объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="55011-116">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="55011-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="55011-117">Определяет идентификатор элемента объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="55011-118">Словарь</span><span class="sxs-lookup"><span data-stu-id="55011-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="55011-119">Определяет набор записи словаря свойства для объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="55011-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="55011-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="55011-121">Содержит контент свойства XML данных для объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="55011-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="55011-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="55011-123">Свойство содержимым для объекта конфигурации пользователя двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="55011-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55011-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55011-124">Parent elements</span></span>

|<span data-ttu-id="55011-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55011-125">**Element**</span></span>|<span data-ttu-id="55011-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55011-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55011-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55011-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="55011-128">Представляет запрос на создание объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="55011-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="55011-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="55011-130">Представляет ответа, которое возвращает объект конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="55011-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55011-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="55011-132">Представляет запрос на обновление объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="55011-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55011-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="55011-133">Remarks</span></span>

<span data-ttu-id="55011-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="55011-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55011-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55011-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55011-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55011-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55011-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55011-137">Schema Name</span></span>  <br/> |<span data-ttu-id="55011-138">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="55011-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55011-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55011-139">Validation File</span></span>  <br/> |<span data-ttu-id="55011-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55011-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55011-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55011-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="55011-142">False</span><span class="sxs-lookup"><span data-stu-id="55011-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55011-143">См. также</span><span class="sxs-lookup"><span data-stu-id="55011-143">See also</span></span>



- [<span data-ttu-id="55011-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="55011-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
