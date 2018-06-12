---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: Элемент DelegationState представляет состояние делегированные задачи.
ms.openlocfilehash: 00b0e41ae223f1c70f9a3a21662e8858f8690a86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762014"
---
# <a name="delegationstate"></a><span data-ttu-id="0aca4-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="0aca4-103">DelegationState</span></span>

<span data-ttu-id="0aca4-104">Элемент **DelegationState** представляет состояние делегированные задачи.</span><span class="sxs-lookup"><span data-stu-id="0aca4-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="0aca4-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="0aca4-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0aca4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0aca4-106">Attributes and elements</span></span>

<span data-ttu-id="0aca4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0aca4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0aca4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0aca4-108">Attributes</span></span>

<span data-ttu-id="0aca4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0aca4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0aca4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0aca4-110">Child elements</span></span>

<span data-ttu-id="0aca4-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0aca4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0aca4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0aca4-112">Parent elements</span></span>

|<span data-ttu-id="0aca4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0aca4-113">**Element**</span></span>|<span data-ttu-id="0aca4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0aca4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aca4-115">Задача</span><span class="sxs-lookup"><span data-stu-id="0aca4-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="0aca4-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0aca4-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0aca4-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0aca4-117">Text value</span></span>

<span data-ttu-id="0aca4-118">Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0aca4-118">This is a read-only property.</span></span> <span data-ttu-id="0aca4-119">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="0aca4-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="0aca4-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="0aca4-120">NoMatch</span></span>
    
- <span data-ttu-id="0aca4-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="0aca4-121">OwnNew</span></span>
    
- <span data-ttu-id="0aca4-122">Владельцем</span><span class="sxs-lookup"><span data-stu-id="0aca4-122">Owned</span></span>
    
- <span data-ttu-id="0aca4-123">Принято</span><span class="sxs-lookup"><span data-stu-id="0aca4-123">Accepted</span></span>
    
- <span data-ttu-id="0aca4-124">Отклонено</span><span class="sxs-lookup"><span data-stu-id="0aca4-124">Declined</span></span>
    
- <span data-ttu-id="0aca4-125">Max</span><span class="sxs-lookup"><span data-stu-id="0aca4-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0aca4-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="0aca4-126">Remarks</span></span>

<span data-ttu-id="0aca4-127">Веб-служб Exchange в Microsoft Exchange Server 2007 не поддерживает назначений задач.</span><span class="sxs-lookup"><span data-stu-id="0aca4-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="0aca4-128">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="0aca4-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0aca4-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0aca4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0aca4-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0aca4-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0aca4-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0aca4-131">Schema Name</span></span>  <br/> |<span data-ttu-id="0aca4-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0aca4-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="0aca4-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0aca4-133">Validation File</span></span>  <br/> |<span data-ttu-id="0aca4-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0aca4-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0aca4-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0aca4-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="0aca4-136">False</span><span class="sxs-lookup"><span data-stu-id="0aca4-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0aca4-137">См. также</span><span class="sxs-lookup"><span data-stu-id="0aca4-137">See also</span></span>

- [<span data-ttu-id="0aca4-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0aca4-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
