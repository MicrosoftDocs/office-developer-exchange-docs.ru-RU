---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: Элемент ToRecipients содержит массив получателей элемента. Далее представлены основные получателей элемента.
ms.openlocfilehash: 2913705cad52c041809769fe58efc3d616f40462
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840215"
---
# <a name="torecipients"></a><span data-ttu-id="a0d5e-104">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="a0d5e-104">ToRecipients</span></span>

<span data-ttu-id="a0d5e-p102">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **ToRecipients** содержит массив получателей элемента. Далее представлены основные получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-p102">The **ToRecipients** element contains an array of recipients of an item. These are the primary recipients of an item.</span></span> 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 <span data-ttu-id="a0d5e-107">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="a0d5e-107">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0d5e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a0d5e-108">Attributes and elements</span></span>

<span data-ttu-id="a0d5e-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0d5e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a0d5e-110">Attributes</span></span>

<span data-ttu-id="a0d5e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0d5e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a0d5e-112">Child elements</span></span>

|<span data-ttu-id="a0d5e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0d5e-113">**Element**</span></span>|<span data-ttu-id="a0d5e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0d5e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0d5e-115">Mailbox</span><span class="sxs-lookup"><span data-stu-id="a0d5e-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="a0d5e-116">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0d5e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a0d5e-117">Parent elements</span></span>

|<span data-ttu-id="a0d5e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0d5e-118">**Element**</span></span>|<span data-ttu-id="a0d5e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0d5e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0d5e-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="a0d5e-121">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-122">Message</span><span class="sxs-lookup"><span data-stu-id="a0d5e-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a0d5e-123">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-124">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="a0d5e-124">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="a0d5e-125">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-125">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a0d5e-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a0d5e-127">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-128">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a0d5e-128">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="a0d5e-129">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-129">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="a0d5e-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="a0d5e-131">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-132">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-132">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="a0d5e-133">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-133">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-134">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-134">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="a0d5e-135">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-135">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-136">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-136">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="a0d5e-137">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-137">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-138">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-138">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="a0d5e-139">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-139">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-140">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-140">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="a0d5e-141">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-141">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-142">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-142">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="a0d5e-143">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-143">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="a0d5e-144">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="a0d5e-144">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="a0d5e-145">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-145">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0d5e-146">Замечания</span><span class="sxs-lookup"><span data-stu-id="a0d5e-146">Remarks</span></span>

<span data-ttu-id="a0d5e-p103">Не удается получить **ToRecipients** с помощью запроса FindItem. Используйте GetItem запрос для получения **ToRecipients**.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-p103">You cannot get **ToRecipients** by using a FindItem request. Use a GetItem request to get the **ToRecipients**.</span></span>
  
<span data-ttu-id="a0d5e-149">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a0d5e-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0d5e-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a0d5e-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0d5e-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a0d5e-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0d5e-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a0d5e-152">Schema Name</span></span>  <br/> |<span data-ttu-id="a0d5e-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a0d5e-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0d5e-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a0d5e-154">Validation File</span></span>  <br/> |<span data-ttu-id="a0d5e-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0d5e-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0d5e-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a0d5e-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0d5e-157">False</span><span class="sxs-lookup"><span data-stu-id="a0d5e-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0d5e-158">См. также</span><span class="sxs-lookup"><span data-stu-id="a0d5e-158">See also</span></span>



- [<span data-ttu-id="a0d5e-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a0d5e-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
