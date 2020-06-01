---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: Элемент FindConversation определяет запрос на поиск бесед в почтовом ящике.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462649"
---
# <a name="findconversation"></a><span data-ttu-id="74ea3-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="74ea3-103">FindConversation</span></span>

<span data-ttu-id="74ea3-104">Элемент **FindConversation** определяет запрос на поиск бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="74ea3-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="74ea3-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="74ea3-105">FindConversation</span></span>](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 <span data-ttu-id="74ea3-106">**финдконверсатионтипе**</span><span class="sxs-lookup"><span data-stu-id="74ea3-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74ea3-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74ea3-107">Attributes and elements</span></span>

<span data-ttu-id="74ea3-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="74ea3-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74ea3-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74ea3-109">Attributes</span></span>

****

|<span data-ttu-id="74ea3-110">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="74ea3-110">**Attribute**</span></span>|<span data-ttu-id="74ea3-111">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74ea3-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74ea3-112">Обход</span><span class="sxs-lookup"><span data-stu-id="74ea3-112">Traversal</span></span>  <br/> |<span data-ttu-id="74ea3-113">Определяет типы обхода вложенного дерева.</span><span class="sxs-lookup"><span data-stu-id="74ea3-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="74ea3-114">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="74ea3-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="74ea3-115">виевфилтер</span><span class="sxs-lookup"><span data-stu-id="74ea3-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="74ea3-116">Определяет фильтры представления типов.</span><span class="sxs-lookup"><span data-stu-id="74ea3-116">Identifies the types view filters.</span></span> <span data-ttu-id="74ea3-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="74ea3-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="74ea3-118">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="74ea3-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="74ea3-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="74ea3-119">**Value**</span></span>|<span data-ttu-id="74ea3-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74ea3-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74ea3-121">Поверхност</span><span class="sxs-lookup"><span data-stu-id="74ea3-121">Shallow</span></span>  <br/> |<span data-ttu-id="74ea3-122">Обозначает неполную обходов.</span><span class="sxs-lookup"><span data-stu-id="74ea3-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="74ea3-123">Углублен</span><span class="sxs-lookup"><span data-stu-id="74ea3-123">Deep</span></span>  <br/> |<span data-ttu-id="74ea3-124">Указывает на глубокий обход.</span><span class="sxs-lookup"><span data-stu-id="74ea3-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="74ea3-125">Значения атрибутов Виевфилтер</span><span class="sxs-lookup"><span data-stu-id="74ea3-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="74ea3-126">**Значение**</span><span class="sxs-lookup"><span data-stu-id="74ea3-126">**Value**</span></span>|<span data-ttu-id="74ea3-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74ea3-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74ea3-128">Все</span><span class="sxs-lookup"><span data-stu-id="74ea3-128">All</span></span>  <br/> |<span data-ttu-id="74ea3-129">Поиск всех бесед.</span><span class="sxs-lookup"><span data-stu-id="74ea3-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="74ea3-130">Отмеченные</span><span class="sxs-lookup"><span data-stu-id="74ea3-130">Flagged</span></span>  <br/> |<span data-ttu-id="74ea3-131">Поиск помеченных бесед.</span><span class="sxs-lookup"><span data-stu-id="74ea3-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="74ea3-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="74ea3-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="74ea3-133">Поиск бесед с вложениями.</span><span class="sxs-lookup"><span data-stu-id="74ea3-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="74ea3-134">турккме</span><span class="sxs-lookup"><span data-stu-id="74ea3-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="74ea3-135">Поиск бесед, адресованных или получателей CC.</span><span class="sxs-lookup"><span data-stu-id="74ea3-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="74ea3-136">Unread</span><span class="sxs-lookup"><span data-stu-id="74ea3-136">Unread</span></span>  <br/> |<span data-ttu-id="74ea3-137">Поиск непрочитанных бесед.</span><span class="sxs-lookup"><span data-stu-id="74ea3-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="74ea3-138">таскактиве</span><span class="sxs-lookup"><span data-stu-id="74ea3-138">TaskActive</span></span>  <br/> |<span data-ttu-id="74ea3-139">Поиск активных задач.</span><span class="sxs-lookup"><span data-stu-id="74ea3-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="74ea3-140">тасковердуе</span><span class="sxs-lookup"><span data-stu-id="74ea3-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="74ea3-141">Поиск просроченных задач.</span><span class="sxs-lookup"><span data-stu-id="74ea3-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="74ea3-142">тасккомплетед</span><span class="sxs-lookup"><span data-stu-id="74ea3-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="74ea3-143">Поиск завершенных задач.</span><span class="sxs-lookup"><span data-stu-id="74ea3-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="74ea3-144">Функция "несрочные"</span><span class="sxs-lookup"><span data-stu-id="74ea3-144">NoClutter</span></span>  <br/> |<span data-ttu-id="74ea3-145">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="74ea3-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="74ea3-146">Папка "Несрочные"</span><span class="sxs-lookup"><span data-stu-id="74ea3-146">Clutter</span></span>  <br/> |<span data-ttu-id="74ea3-147">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="74ea3-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="74ea3-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74ea3-148">Child elements</span></span>

|<span data-ttu-id="74ea3-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="74ea3-149">**Element**</span></span>|<span data-ttu-id="74ea3-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74ea3-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74ea3-151">индекседпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="74ea3-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="74ea3-152">Описывает, как возвращаются сведения о страничной беседе.</span><span class="sxs-lookup"><span data-stu-id="74ea3-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="74ea3-153">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="74ea3-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="74ea3-154">Задает условие, используемое для определения конца поиска, начального индекса поиска, максимальных возвращаемых значений и направления поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="74ea3-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="74ea3-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="74ea3-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="74ea3-156">Определяет порядок сортировки элементов в запросе [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="74ea3-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="74ea3-157">Свойство **CONVERSATION: ластделиверитиме** — единственное свойство, которое поддерживается для сортировки при использовании операции **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="74ea3-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="74ea3-158">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="74ea3-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="74ea3-159">Определяет папку для поиска обсуждений.</span><span class="sxs-lookup"><span data-stu-id="74ea3-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="74ea3-160">маилбоксскопе</span><span class="sxs-lookup"><span data-stu-id="74ea3-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="74ea3-161">Указывает, следует ли выполнять поиск или выборку для беседы: в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="74ea3-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="74ea3-162">Строка запроса (Куеристрингтипе)</span><span class="sxs-lookup"><span data-stu-id="74ea3-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="74ea3-163">Указывает строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).</span><span class="sxs-lookup"><span data-stu-id="74ea3-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="74ea3-164">конверсатионшапе</span><span class="sxs-lookup"><span data-stu-id="74ea3-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="74ea3-165">Определяет значение свойства, возвращаемого в ответе [операции FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="74ea3-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74ea3-166">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74ea3-166">Parent elements</span></span>

<span data-ttu-id="74ea3-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="74ea3-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74ea3-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="74ea3-168">Remarks</span></span>

<span data-ttu-id="74ea3-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="74ea3-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74ea3-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74ea3-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74ea3-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74ea3-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74ea3-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74ea3-172">Schema Name</span></span>  <br/> |<span data-ttu-id="74ea3-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="74ea3-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74ea3-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74ea3-174">Validation File</span></span>  <br/> |<span data-ttu-id="74ea3-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74ea3-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74ea3-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74ea3-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="74ea3-177">False</span><span class="sxs-lookup"><span data-stu-id="74ea3-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74ea3-178">См. также</span><span class="sxs-lookup"><span data-stu-id="74ea3-178">See also</span></span>



[<span data-ttu-id="74ea3-179">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="74ea3-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="74ea3-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="74ea3-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="74ea3-181">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="74ea3-181">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

