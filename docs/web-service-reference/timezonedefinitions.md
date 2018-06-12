---
title: TimeZoneDefinitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinitions
api_type:
- schema
ms.assetid: 9ca1584e-65b8-49ba-a408-e3e8597e6607
description: Элемент TimeZoneDefinitions представляет собой массив из определения часового пояса.
ms.openlocfilehash: 0bc1b69ef564bb4e239d9845a4b1a0133292ff12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840190"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="77969-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="77969-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="77969-104">Элемент **TimeZoneDefinitions** представляет собой массив из определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="77969-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="77969-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="77969-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77969-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77969-106">Attributes and elements</span></span>

<span data-ttu-id="77969-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="77969-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77969-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77969-108">Attributes</span></span>

<span data-ttu-id="77969-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="77969-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77969-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77969-110">Child elements</span></span>

|<span data-ttu-id="77969-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77969-111">**Element**</span></span>|<span data-ttu-id="77969-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77969-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77969-113">Определение часового пояса</span><span class="sxs-lookup"><span data-stu-id="77969-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="77969-114">Задает периодов и переходы, определяющие часового пояса.</span><span class="sxs-lookup"><span data-stu-id="77969-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77969-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77969-115">Parent elements</span></span>

|<span data-ttu-id="77969-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77969-116">**Element**</span></span>|<span data-ttu-id="77969-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77969-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77969-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77969-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="77969-119">Содержит состояние и результат [операции GetServerTimeZones](getservertimezones-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="77969-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77969-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="77969-120">Remarks</span></span>

<span data-ttu-id="77969-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77969-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77969-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77969-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77969-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77969-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77969-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77969-124">Schema Name</span></span>  <br/> |<span data-ttu-id="77969-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="77969-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77969-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77969-126">Validation File</span></span>  <br/> |<span data-ttu-id="77969-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77969-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77969-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77969-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="77969-129">False</span><span class="sxs-lookup"><span data-stu-id="77969-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77969-130">См. также</span><span class="sxs-lookup"><span data-stu-id="77969-130">See also</span></span>



- [<span data-ttu-id="77969-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="77969-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

