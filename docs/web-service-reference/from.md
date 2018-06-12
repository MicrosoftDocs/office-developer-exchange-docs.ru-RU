---
title: From
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: Элемент From представляет адрес, с которого было отправлено сообщение.
ms.openlocfilehash: 39c8c8ef84ff445e8f44ebb9f2285ccfc42353a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762670"
---
# <a name="from"></a><span data-ttu-id="6990e-103">From</span><span class="sxs-lookup"><span data-stu-id="6990e-103">From</span></span>

<span data-ttu-id="6990e-104">Элемент **из** представляет адрес, с которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="6990e-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="6990e-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="6990e-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6990e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6990e-106">Attributes and elements</span></span>

<span data-ttu-id="6990e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6990e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6990e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6990e-108">Attributes</span></span>

<span data-ttu-id="6990e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6990e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6990e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6990e-110">Child elements</span></span>

|<span data-ttu-id="6990e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6990e-111">**Element**</span></span>|<span data-ttu-id="6990e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6990e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6990e-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="6990e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="6990e-114">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6990e-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6990e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6990e-115">Parent elements</span></span>

|<span data-ttu-id="6990e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6990e-116">**Element**</span></span>|<span data-ttu-id="6990e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6990e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6990e-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="6990e-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="6990e-119">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-120">Message</span><span class="sxs-lookup"><span data-stu-id="6990e-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6990e-121">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6990e-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="6990e-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6990e-123">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6990e-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6990e-125">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6990e-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6990e-127">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="6990e-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6990e-129">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="6990e-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="6990e-131">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="6990e-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6990e-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="6990e-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="6990e-133">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6990e-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6990e-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="6990e-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="6990e-135">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="6990e-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6990e-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="6990e-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="6990e-137">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="6990e-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="6990e-139">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6990e-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="6990e-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="6990e-141">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="6990e-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="6990e-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="6990e-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="6990e-143">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="6990e-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6990e-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="6990e-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="6990e-145">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6990e-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="6990e-146">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6990e-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6990e-147">Замечания</span><span class="sxs-lookup"><span data-stu-id="6990e-147">Remarks</span></span>

<span data-ttu-id="6990e-148">Данный элемент используется для сообщений электронной почты «отправить от имени».</span><span class="sxs-lookup"><span data-stu-id="6990e-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="6990e-149">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6990e-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6990e-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6990e-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6990e-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6990e-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6990e-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6990e-152">Schema Name</span></span>  <br/> |<span data-ttu-id="6990e-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6990e-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="6990e-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6990e-154">Validation File</span></span>  <br/> |<span data-ttu-id="6990e-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6990e-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6990e-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6990e-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="6990e-157">False</span><span class="sxs-lookup"><span data-stu-id="6990e-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6990e-158">См. также</span><span class="sxs-lookup"><span data-stu-id="6990e-158">See also</span></span>



- [<span data-ttu-id="6990e-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6990e-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
