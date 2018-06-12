---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: Элемент GetConversationItems определяет запрос на получение набора элементов, которые связаны, не упустив в одной беседе.
ms.openlocfilehash: 9be300318a07173e4a8e11e5a6ca78b885de1199
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762722"
---
# <a name="getconversationitems"></a><span data-ttu-id="4c935-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="4c935-103">GetConversationItems</span></span>

<span data-ttu-id="4c935-104">Элемент **GetConversationItems** определяет запрос на получение набора элементов, которые связаны, не упустив в одной беседе.</span><span class="sxs-lookup"><span data-stu-id="4c935-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 <span data-ttu-id="4c935-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="4c935-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c935-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4c935-106">Attributes and elements</span></span>

<span data-ttu-id="4c935-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4c935-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c935-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4c935-108">Attributes</span></span>

<span data-ttu-id="4c935-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c935-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c935-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4c935-110">Child elements</span></span>

<span data-ttu-id="4c935-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [бесед](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="4c935-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c935-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4c935-112">Parent elements</span></span>

<span data-ttu-id="4c935-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c935-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c935-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="4c935-114">Remarks</span></span>

<span data-ttu-id="4c935-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4c935-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c935-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c935-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c935-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4c935-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c935-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4c935-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4c935-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4c935-119">Schema name</span></span>  <br/> |<span data-ttu-id="4c935-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4c935-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4c935-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4c935-121">Validation file</span></span>  <br/> |<span data-ttu-id="4c935-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4c935-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4c935-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4c935-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4c935-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4c935-124">false</span></span>  <br/> |
   

