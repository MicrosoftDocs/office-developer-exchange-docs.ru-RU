---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: Элемент PullSubscriptionRequest — подписка на подписку на уведомления о событий на основе репликации по запросу.
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834932"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="db43b-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="db43b-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="db43b-104">Элемент **PullSubscriptionRequest** — подписка на подписку на уведомления о событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="db43b-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="db43b-105">Подписка</span><span class="sxs-lookup"><span data-stu-id="db43b-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="db43b-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="db43b-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="db43b-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="db43b-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db43b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db43b-108">Attributes and elements</span></span>

<span data-ttu-id="db43b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="db43b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db43b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db43b-110">Attributes</span></span>

|<span data-ttu-id="db43b-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="db43b-111">**Attribute**</span></span>|<span data-ttu-id="db43b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db43b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db43b-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="db43b-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="db43b-114">Указывает, следует ли подписка на всех доступных папок.</span><span class="sxs-lookup"><span data-stu-id="db43b-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="db43b-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="db43b-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="db43b-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db43b-116">Child elements</span></span>

|<span data-ttu-id="db43b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db43b-117">**Element**</span></span>|<span data-ttu-id="db43b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db43b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db43b-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="db43b-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="db43b-120">Содержит массив идентификаторов папок, которые используются для определения папок для наблюдения за уведомления о событиях.</span><span class="sxs-lookup"><span data-stu-id="db43b-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="db43b-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="db43b-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="db43b-122">Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="db43b-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="db43b-123">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="db43b-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="db43b-124">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="db43b-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="db43b-125">Используется для создания подписки, начинающимся на события, представленного водяного знака.</span><span class="sxs-lookup"><span data-stu-id="db43b-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="db43b-126">Если водяного знака из подписки на запрос не найден, возврату ошибки будут возвращены клиенту.</span><span class="sxs-lookup"><span data-stu-id="db43b-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="db43b-127">Эта ошибка может возникнуть, если водяной знак старше 30 дней или если водяного знака никогда не был указан в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="db43b-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="db43b-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="db43b-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="db43b-129">Представляет продолжительность в минутах, подписки может простаивать без запроса GetEvents от клиента.</span><span class="sxs-lookup"><span data-stu-id="db43b-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db43b-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db43b-130">Parent elements</span></span>

|<span data-ttu-id="db43b-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db43b-131">**Element**</span></span>|<span data-ttu-id="db43b-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db43b-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db43b-133">Подписка</span><span class="sxs-lookup"><span data-stu-id="db43b-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="db43b-134">Содержит свойства, используемые для создания подписок.</span><span class="sxs-lookup"><span data-stu-id="db43b-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db43b-135">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="db43b-135">Text value</span></span>

<span data-ttu-id="db43b-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="db43b-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db43b-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="db43b-137">Remarks</span></span>

<span data-ttu-id="db43b-138">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="db43b-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db43b-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db43b-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db43b-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db43b-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db43b-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db43b-141">Schema name</span></span>  <br/> |<span data-ttu-id="db43b-142">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="db43b-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db43b-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db43b-143">Validation file</span></span>  <br/> |<span data-ttu-id="db43b-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db43b-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db43b-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db43b-145">Can be empty</span></span>  <br/> |<span data-ttu-id="db43b-146">False</span><span class="sxs-lookup"><span data-stu-id="db43b-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db43b-147">См. также</span><span class="sxs-lookup"><span data-stu-id="db43b-147">See also</span></span>



[<span data-ttu-id="db43b-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="db43b-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="db43b-149">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="db43b-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="db43b-150">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="db43b-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="db43b-151">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="db43b-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="db43b-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="db43b-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
