---
title: IsGreaterThanOrEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThanOrEqualTo
api_type:
- schema
ms.assetid: 373cc954-314d-40e2-be03-cc08aefc0d5b
description: Элемент IsGreaterThanOrEqualTo представляет выражение поиска, которое сравнивает свойство с постоянным значением или другого свойства и возвращает значение true, если первое свойство больше или равен ему.
ms.openlocfilehash: 81df79d15e6c5c8d301e69a822d038588ce42325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834030"
---
# <a name="isgreaterthanorequalto"></a><span data-ttu-id="666d9-103">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="666d9-103">IsGreaterThanOrEqualTo</span></span>

<span data-ttu-id="666d9-104">Элемент **IsGreaterThanOrEqualTo** представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает **значение true,** Если первое свойство больше или равен ему.</span><span class="sxs-lookup"><span data-stu-id="666d9-104">The **IsGreaterThanOrEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the second.</span></span> 
  
```xml
<IsGreaterThanOrEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThanOrEqualTo>
```

 <span data-ttu-id="666d9-105">**IsGreaterThanOrEqualToType**</span><span class="sxs-lookup"><span data-stu-id="666d9-105">**IsGreaterThanOrEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="666d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="666d9-106">Attributes and elements</span></span>

<span data-ttu-id="666d9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="666d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="666d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="666d9-108">Attributes</span></span>

<span data-ttu-id="666d9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="666d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="666d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="666d9-110">Child elements</span></span>

|<span data-ttu-id="666d9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="666d9-111">**Element**</span></span>|<span data-ttu-id="666d9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="666d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="666d9-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="666d9-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="666d9-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="666d9-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="666d9-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="666d9-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="666d9-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="666d9-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="666d9-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="666d9-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="666d9-118">Задает свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="666d9-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="666d9-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="666d9-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="666d9-120">Представляет свойство или постоянное значение для использования при сравнении с другого свойства.</span><span class="sxs-lookup"><span data-stu-id="666d9-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="666d9-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="666d9-121">Parent elements</span></span>

|<span data-ttu-id="666d9-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="666d9-122">**Element**</span></span>|<span data-ttu-id="666d9-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="666d9-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="666d9-124">Ограничения</span><span class="sxs-lookup"><span data-stu-id="666d9-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="666d9-125">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.</span><span class="sxs-lookup"><span data-stu-id="666d9-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="666d9-126">Не</span><span class="sxs-lookup"><span data-stu-id="666d9-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="666d9-127">Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="666d9-127">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="666d9-128">И</span><span class="sxs-lookup"><span data-stu-id="666d9-128">And</span></span>](and.md) <br/> |<span data-ttu-id="666d9-129">Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска.</span><span class="sxs-lookup"><span data-stu-id="666d9-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="666d9-130">Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.</span><span class="sxs-lookup"><span data-stu-id="666d9-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="666d9-131">Или</span><span class="sxs-lookup"><span data-stu-id="666d9-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="666d9-132">Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит.</span><span class="sxs-lookup"><span data-stu-id="666d9-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="666d9-133">[Или](or.md) возвращает значение true, если какие-либо из их дочерних элементов возвращало значение true.</span><span class="sxs-lookup"><span data-stu-id="666d9-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="666d9-134">[Или](or.md) должен иметь два или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="666d9-134">[Or](or.md) must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="666d9-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="666d9-135">Remarks</span></span>

<span data-ttu-id="666d9-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="666d9-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="666d9-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="666d9-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="666d9-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="666d9-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="666d9-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="666d9-139">Schema Name</span></span>  <br/> |<span data-ttu-id="666d9-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="666d9-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="666d9-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="666d9-141">Validation File</span></span>  <br/> |<span data-ttu-id="666d9-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="666d9-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="666d9-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="666d9-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="666d9-144">False</span><span class="sxs-lookup"><span data-stu-id="666d9-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="666d9-145">См. также</span><span class="sxs-lookup"><span data-stu-id="666d9-145">See also</span></span>



- [<span data-ttu-id="666d9-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="666d9-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
