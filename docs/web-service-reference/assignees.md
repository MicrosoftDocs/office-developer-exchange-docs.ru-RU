---
title: Assignees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: Элемент Assignees указывает людей, которому назначена задача.
ms.openlocfilehash: 5fc301cd77268213e95fd33a2a2f36dbe218b512
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761501"
---
# <a name="assignees"></a><span data-ttu-id="d3c39-103">Assignees</span><span class="sxs-lookup"><span data-stu-id="d3c39-103">Assignees</span></span>

<span data-ttu-id="d3c39-104">Элемент **Assignees** указывает людей, которому назначена задача.</span><span class="sxs-lookup"><span data-stu-id="d3c39-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="d3c39-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="d3c39-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3c39-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3c39-106">Attributes and elements</span></span>

<span data-ttu-id="d3c39-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d3c39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3c39-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3c39-108">Attributes</span></span>

<span data-ttu-id="d3c39-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3c39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3c39-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3c39-110">Child elements</span></span>

|<span data-ttu-id="d3c39-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3c39-111">**Element**</span></span>|<span data-ttu-id="d3c39-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3c39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3c39-113">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d3c39-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="d3c39-114">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3c39-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d3c39-115">Идентификатор пользователя (строка)</span><span class="sxs-lookup"><span data-stu-id="d3c39-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="d3c39-116">Задает идентификатор пользователя для пользователя по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="d3c39-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3c39-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3c39-117">Parent elements</span></span>

|<span data-ttu-id="d3c39-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3c39-118">**Element**</span></span>|<span data-ttu-id="d3c39-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3c39-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3c39-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="d3c39-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="d3c39-121">Задает предложенная задача.</span><span class="sxs-lookup"><span data-stu-id="d3c39-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3c39-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3c39-122">Remarks</span></span>

<span data-ttu-id="d3c39-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d3c39-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d3c39-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3c39-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3c39-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3c39-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3c39-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3c39-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3c39-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3c39-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d3c39-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d3c39-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="d3c39-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3c39-129">Validation File</span></span>  <br/> |<span data-ttu-id="d3c39-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3c39-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3c39-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3c39-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d3c39-132">См. также</span><span class="sxs-lookup"><span data-stu-id="d3c39-132">See also</span></span>

- [<span data-ttu-id="d3c39-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d3c39-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
