---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: Элемент GlobalLastDeliveryTime содержит время доставки сообщений, который был получен последний беседы во всех папках в почтовом ящике.
ms.openlocfilehash: fded5cd1891a406f0979cf4bec7321779d70ab3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833733"
---
# <a name="globallastdeliverytime"></a><span data-ttu-id="03864-103">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="03864-103">GlobalLastDeliveryTime</span></span>

<span data-ttu-id="03864-104">Элемент **GlobalLastDeliveryTime** содержит время доставки сообщений, который был получен последний беседы во всех папках в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="03864-104">The **GlobalLastDeliveryTime** element contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="03864-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="03864-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="03864-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="03864-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="03864-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="03864-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="03864-108">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="03864-108">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 <span data-ttu-id="03864-109">**xs: DateTime**</span><span class="sxs-lookup"><span data-stu-id="03864-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03864-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03864-110">Attributes and elements</span></span>

<span data-ttu-id="03864-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="03864-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03864-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03864-112">Attributes</span></span>

<span data-ttu-id="03864-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="03864-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03864-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03864-114">Child elements</span></span>

<span data-ttu-id="03864-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="03864-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03864-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03864-116">Parent elements</span></span>

|<span data-ttu-id="03864-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03864-117">**Element**</span></span>|<span data-ttu-id="03864-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03864-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03864-119">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="03864-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="03864-120">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="03864-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03864-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="03864-121">Text value</span></span>

<span data-ttu-id="03864-122">Текстовое значение элемента **GlobalLastDeliveryTime** — это дата и время сообщения, который был получен последний беседы во всех папках в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="03864-122">The text value of the **GlobalLastDeliveryTime** element is the date and time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="03864-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="03864-123">Remarks</span></span>

<span data-ttu-id="03864-124">Этот элемент был представлен в пакете обновления 1 (SP1) для Exchange Server 2010. Схема, описывающая этот элемент находится в виртуальном каталоге IIS, на котором размещается веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="03864-124">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03864-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="03864-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03864-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="03864-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03864-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="03864-127">Schema name</span></span>  <br/> |<span data-ttu-id="03864-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="03864-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="03864-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="03864-129">Validation file</span></span>  <br/> |<span data-ttu-id="03864-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03864-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03864-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="03864-131">Can be empty</span></span>  <br/> |<span data-ttu-id="03864-132">False</span><span class="sxs-lookup"><span data-stu-id="03864-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03864-133">См. также</span><span class="sxs-lookup"><span data-stu-id="03864-133">See also</span></span>



[<span data-ttu-id="03864-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="03864-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="03864-135">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="03864-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="03864-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="03864-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

