---
title: ResponseObjects
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: Элемент ResponseObjects содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.
ms.openlocfilehash: b1d95063439f5089665d2aad97d747665caef0ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835197"
---
# <a name="responseobjects"></a><span data-ttu-id="77ce4-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="77ce4-103">ResponseObjects</span></span>

<span data-ttu-id="77ce4-104">Элемент **ResponseObjects** содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 <span data-ttu-id="77ce4-105">**NonEmptyArrayOfResponseObjectsType**</span><span class="sxs-lookup"><span data-stu-id="77ce4-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77ce4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="77ce4-106">Attributes and elements</span></span>

<span data-ttu-id="77ce4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="77ce4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77ce4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="77ce4-108">Attributes</span></span>

<span data-ttu-id="77ce4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="77ce4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77ce4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="77ce4-110">Child elements</span></span>

|<span data-ttu-id="77ce4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77ce4-111">**Element**</span></span>|<span data-ttu-id="77ce4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77ce4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77ce4-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="77ce4-114">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="77ce4-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="77ce4-116">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="77ce4-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="77ce4-118">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="77ce4-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="77ce4-120">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-121">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="77ce4-122">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="77ce4-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-123">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="77ce4-124">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="77ce4-126">Представляет объект ответа, используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="77ce4-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="77ce4-128">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="77ce4-130">Содержит ответ элемента записи.</span><span class="sxs-lookup"><span data-stu-id="77ce4-130">Contains a reply to a post item.</span></span> <span data-ttu-id="77ce4-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="77ce4-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="77ce4-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="77ce4-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="77ce4-133">Используется для отмены вывода прочтении запросов.</span><span class="sxs-lookup"><span data-stu-id="77ce4-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-134">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="77ce4-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="77ce4-135">Используется для принятия приглашения, которая позволяет получить доступ к календарю другого пользователя или данных контактов.</span><span class="sxs-lookup"><span data-stu-id="77ce4-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77ce4-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="77ce4-136">Parent elements</span></span>

|<span data-ttu-id="77ce4-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="77ce4-137">**Element**</span></span>|<span data-ttu-id="77ce4-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="77ce4-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77ce4-139">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="77ce4-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="77ce4-140">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-141">Контакт</span><span class="sxs-lookup"><span data-stu-id="77ce4-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="77ce4-142">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="77ce4-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="77ce4-144">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="77ce4-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-145">Элемент</span><span class="sxs-lookup"><span data-stu-id="77ce4-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="77ce4-146">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="77ce4-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="77ce4-148">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="77ce4-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="77ce4-150">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="77ce4-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="77ce4-152">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="77ce4-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="77ce4-154">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-155">Message</span><span class="sxs-lookup"><span data-stu-id="77ce4-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77ce4-156">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="77ce4-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="77ce4-158">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77ce4-159">Задача</span><span class="sxs-lookup"><span data-stu-id="77ce4-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="77ce4-160">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77ce4-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="77ce4-161">Remarks</span></span>

<span data-ttu-id="77ce4-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="77ce4-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77ce4-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="77ce4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77ce4-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="77ce4-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77ce4-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="77ce4-165">Schema Name</span></span>  <br/> |<span data-ttu-id="77ce4-166">Схема Types</span><span class="sxs-lookup"><span data-stu-id="77ce4-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="77ce4-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="77ce4-167">Validation File</span></span>  <br/> |<span data-ttu-id="77ce4-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="77ce4-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77ce4-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="77ce4-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="77ce4-170">False</span><span class="sxs-lookup"><span data-stu-id="77ce4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77ce4-171">См. также</span><span class="sxs-lookup"><span data-stu-id="77ce4-171">See also</span></span>



- [<span data-ttu-id="77ce4-172">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="77ce4-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
