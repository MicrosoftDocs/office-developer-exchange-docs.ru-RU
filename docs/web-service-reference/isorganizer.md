---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: Элемент IsOrganizer задает логическое значение, указывающее, является ли этот человек организатора собрания.
ms.openlocfilehash: 5fd775cfc0a296c08d19d0468d96aa36ba67ddd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834063"
---
# <a name="isorganizer"></a><span data-ttu-id="63e18-103">IsOrganizer</span><span class="sxs-lookup"><span data-stu-id="63e18-103">IsOrganizer</span></span>

<span data-ttu-id="63e18-104">Элемент **IsOrganizer** задает логическое значение, указывающее, является ли этот человек организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="63e18-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="63e18-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="63e18-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63e18-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="63e18-106">Attributes and elements</span></span>

<span data-ttu-id="63e18-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="63e18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63e18-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="63e18-108">Attributes</span></span>

<span data-ttu-id="63e18-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="63e18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63e18-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="63e18-110">Child elements</span></span>

<span data-ttu-id="63e18-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="63e18-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63e18-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="63e18-112">Parent elements</span></span>

|<span data-ttu-id="63e18-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63e18-113">**Element**</span></span>|<span data-ttu-id="63e18-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63e18-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63e18-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="63e18-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="63e18-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="63e18-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="63e18-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="63e18-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="63e18-118">Представляет сообщение собрания.</span><span class="sxs-lookup"><span data-stu-id="63e18-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63e18-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="63e18-119">Text value</span></span>

<span data-ttu-id="63e18-120">Текстовое значение **true** для элемента **IsOrganizer** указывает, что сообщение календаря элемента или собрания была создана пользователем.</span><span class="sxs-lookup"><span data-stu-id="63e18-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="63e18-121">Значение **false** указывает, что сообщение собрание или элемент календаря не было создано bv пользователя.</span><span class="sxs-lookup"><span data-stu-id="63e18-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="63e18-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="63e18-122">Remarks</span></span>

<span data-ttu-id="63e18-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="63e18-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="63e18-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="63e18-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63e18-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="63e18-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63e18-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="63e18-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63e18-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="63e18-127">Schema Name</span></span>  <br/> |<span data-ttu-id="63e18-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="63e18-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="63e18-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="63e18-129">Validation File</span></span>  <br/> |<span data-ttu-id="63e18-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63e18-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="63e18-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="63e18-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="63e18-132">См. также</span><span class="sxs-lookup"><span data-stu-id="63e18-132">See also</span></span>



- [<span data-ttu-id="63e18-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="63e18-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

