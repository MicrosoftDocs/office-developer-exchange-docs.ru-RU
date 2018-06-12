---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: Элемент UserConfigurationProperties Указывает типы свойств для получения в GetUserConfiguration операции.
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840416"
---
# <a name="userconfigurationproperties"></a><span data-ttu-id="68e9a-103">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="68e9a-103">UserConfigurationProperties</span></span>

<span data-ttu-id="68e9a-104">Элемент **UserConfigurationProperties** Указывает типы свойств для получения в GetUserConfiguration операции.</span><span class="sxs-lookup"><span data-stu-id="68e9a-104">The **UserConfigurationProperties** element specifies the property types to get in a GetUserConfiguration operation.</span></span> 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 <span data-ttu-id="68e9a-105">**UserConfigurationPropertyType**</span><span class="sxs-lookup"><span data-stu-id="68e9a-105">**UserConfigurationPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68e9a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68e9a-106">Attributes and elements</span></span>

<span data-ttu-id="68e9a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="68e9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68e9a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68e9a-108">Attributes</span></span>

<span data-ttu-id="68e9a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="68e9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68e9a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68e9a-110">Child elements</span></span>

<span data-ttu-id="68e9a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="68e9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="68e9a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68e9a-112">Parent elements</span></span>

|<span data-ttu-id="68e9a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68e9a-113">**Element**</span></span>|<span data-ttu-id="68e9a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68e9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68e9a-115">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="68e9a-115">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="68e9a-116">Определяет запрос на получение объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="68e9a-116">Specifies a request to get a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68e9a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="68e9a-117">Text value</span></span>

<span data-ttu-id="68e9a-118">В следующей таблице приведены возможные значения для элемента **UserConfigurationProperties** .</span><span class="sxs-lookup"><span data-stu-id="68e9a-118">The following table lists the possible values for the **UserConfigurationProperties** element.</span></span> 
  
|<span data-ttu-id="68e9a-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="68e9a-119">**Value**</span></span>|<span data-ttu-id="68e9a-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68e9a-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68e9a-121">Id</span><span class="sxs-lookup"><span data-stu-id="68e9a-121">Id</span></span>  <br/> |<span data-ttu-id="68e9a-122">Задает свойство идентификатора.</span><span class="sxs-lookup"><span data-stu-id="68e9a-122">Specifies the identifier property.</span></span>  <br/> |
|<span data-ttu-id="68e9a-123">словаря</span><span class="sxs-lookup"><span data-stu-id="68e9a-123">Dictionary</span></span>  <br/> |<span data-ttu-id="68e9a-124">Указывает типы свойств словаря.</span><span class="sxs-lookup"><span data-stu-id="68e9a-124">Specifies dictionary property types.</span></span>  <br/> |
|<span data-ttu-id="68e9a-125">XmlData</span><span class="sxs-lookup"><span data-stu-id="68e9a-125">XmlData</span></span>  <br/> |<span data-ttu-id="68e9a-126">Указывает типы данных свойств XML.</span><span class="sxs-lookup"><span data-stu-id="68e9a-126">Specifies XML data property types.</span></span>  <br/> |
|<span data-ttu-id="68e9a-127">BinaryData</span><span class="sxs-lookup"><span data-stu-id="68e9a-127">BinaryData</span></span>  <br/> |<span data-ttu-id="68e9a-128">Указывает типы свойств двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="68e9a-128">Specifies binary data property types.</span></span>  <br/> |
|<span data-ttu-id="68e9a-129">Все</span><span class="sxs-lookup"><span data-stu-id="68e9a-129">All</span></span>  <br/> |<span data-ttu-id="68e9a-130">Указывает идентификатор, словаря, XML-данных и типы свойств двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="68e9a-130">Specifies the identifier, dictionary, XML data, and binary data property types.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68e9a-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="68e9a-131">Remarks</span></span>

<span data-ttu-id="68e9a-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="68e9a-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68e9a-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68e9a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68e9a-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68e9a-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68e9a-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68e9a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="68e9a-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="68e9a-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68e9a-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68e9a-137">Validation File</span></span>  <br/> |<span data-ttu-id="68e9a-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68e9a-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68e9a-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68e9a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="68e9a-140">False</span><span class="sxs-lookup"><span data-stu-id="68e9a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68e9a-141">См. также</span><span class="sxs-lookup"><span data-stu-id="68e9a-141">See also</span></span>



- [<span data-ttu-id="68e9a-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="68e9a-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
