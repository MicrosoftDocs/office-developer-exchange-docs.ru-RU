---
title: TotalCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TotalCount
api_type:
- schema
ms.assetid: c48c6388-8449-4622-bc38-6f0e84293872
description: Элемент TotalCount — общее количество элементов в указанной папке.
ms.openlocfilehash: e4a7bcb70d04bc5bcf66087c0272732a7be1231a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840217"
---
# <a name="totalcount"></a><span data-ttu-id="06191-103">TotalCount</span><span class="sxs-lookup"><span data-stu-id="06191-103">TotalCount</span></span>

<span data-ttu-id="06191-104">Элемент **TotalCount** — общее количество элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="06191-104">The **TotalCount** element represents the total count of items within a given folder.</span></span> 
  
```xml
<TotalCount/>
```

 <span data-ttu-id="06191-105">**int**</span><span class="sxs-lookup"><span data-stu-id="06191-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06191-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="06191-106">Attributes and elements</span></span>

<span data-ttu-id="06191-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="06191-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06191-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="06191-108">Attributes</span></span>

<span data-ttu-id="06191-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="06191-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06191-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="06191-110">Child elements</span></span>

<span data-ttu-id="06191-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="06191-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06191-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="06191-112">Parent elements</span></span>

|<span data-ttu-id="06191-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06191-113">**Element**</span></span>|<span data-ttu-id="06191-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06191-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06191-115">Folder</span><span class="sxs-lookup"><span data-stu-id="06191-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="06191-116">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="06191-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06191-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="06191-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="06191-118">Представляет папку Календарь в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="06191-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06191-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="06191-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="06191-120">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="06191-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06191-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="06191-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="06191-122">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="06191-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06191-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="06191-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="06191-124">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="06191-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06191-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="06191-125">Text value</span></span>

<span data-ttu-id="06191-126">Текстовое значение представляет собой целое значение.</span><span class="sxs-lookup"><span data-stu-id="06191-126">The text value represents an integer value.</span></span> <span data-ttu-id="06191-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06191-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06191-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="06191-128">Remarks</span></span>

<span data-ttu-id="06191-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="06191-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06191-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="06191-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06191-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="06191-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06191-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="06191-132">Schema Name</span></span>  <br/> |<span data-ttu-id="06191-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="06191-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="06191-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="06191-134">Validation File</span></span>  <br/> |<span data-ttu-id="06191-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="06191-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06191-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="06191-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="06191-137">False</span><span class="sxs-lookup"><span data-stu-id="06191-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06191-138">См. также</span><span class="sxs-lookup"><span data-stu-id="06191-138">See also</span></span>



- [<span data-ttu-id="06191-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="06191-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
