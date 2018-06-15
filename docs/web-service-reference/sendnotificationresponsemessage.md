---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: Элемент SendNotificationResponseMessage содержит состояние и результат одного запроса SendNotification операции.
ms.openlocfilehash: 49677b6d61f525b469679ec3fdcb8aadcca7239d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19835348"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="651c3-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="651c3-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="651c3-104">Элемент **SendNotificationResponseMessage** содержит состояние и результат одного запроса **SendNotification** операции.</span><span class="sxs-lookup"><span data-stu-id="651c3-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="651c3-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="651c3-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="651c3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="651c3-106">Attributes and elements</span></span>

<span data-ttu-id="651c3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="651c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="651c3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="651c3-108">Attributes</span></span>

|<span data-ttu-id="651c3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="651c3-109">**Attribute**</span></span>|<span data-ttu-id="651c3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="651c3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="651c3-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="651c3-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="651c3-112">Описание состояния ответа операции **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="651c3-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="651c3-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="651c3-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="651c3-114">-Success</span><span class="sxs-lookup"><span data-stu-id="651c3-114">-  Success</span></span>  <br/><span data-ttu-id="651c3-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="651c3-115">-  Warning</span></span>  <br/><span data-ttu-id="651c3-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="651c3-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="651c3-117">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="651c3-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="651c3-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="651c3-118">**Value**</span></span>|<span data-ttu-id="651c3-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="651c3-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="651c3-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="651c3-120">**Success**</span></span> <br/> |<span data-ttu-id="651c3-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="651c3-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="651c3-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="651c3-122">**Warning**</span></span> <br/> | <span data-ttu-id="651c3-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="651c3-123">Describes a request that was not processed.</span></span> <span data-ttu-id="651c3-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="651c3-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="651c3-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="651c3-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="651c3-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="651c3-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="651c3-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="651c3-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="651c3-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="651c3-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="651c3-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="651c3-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="651c3-130">-Истек срок действия пароль.</span><span class="sxs-lookup"><span data-stu-id="651c3-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="651c3-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="651c3-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="651c3-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="651c3-132">**Error**</span></span> <br/> | <span data-ttu-id="651c3-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="651c3-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="651c3-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="651c3-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="651c3-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="651c3-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="651c3-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="651c3-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="651c3-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="651c3-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="651c3-138">-Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="651c3-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="651c3-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="651c3-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="651c3-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="651c3-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="651c3-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="651c3-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="651c3-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="651c3-142">Child elements</span></span>

|<span data-ttu-id="651c3-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="651c3-143">**Element**</span></span>|<span data-ttu-id="651c3-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="651c3-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="651c3-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="651c3-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="651c3-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="651c3-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="651c3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="651c3-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="651c3-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="651c3-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="651c3-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="651c3-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="651c3-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="651c3-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="651c3-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="651c3-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="651c3-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="651c3-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="651c3-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="651c3-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="651c3-154">Уведомление</span><span class="sxs-lookup"><span data-stu-id="651c3-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="651c3-155">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="651c3-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="651c3-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="651c3-156">Parent elements</span></span>

|<span data-ttu-id="651c3-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="651c3-157">**Element**</span></span>|<span data-ttu-id="651c3-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="651c3-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="651c3-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="651c3-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="651c3-160">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="651c3-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="651c3-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="651c3-161">Text value</span></span>

<span data-ttu-id="651c3-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="651c3-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="651c3-163">Замечания</span><span class="sxs-lookup"><span data-stu-id="651c3-163">Remarks</span></span>

<span data-ttu-id="651c3-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="651c3-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="651c3-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="651c3-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="651c3-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="651c3-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="651c3-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="651c3-167">Schema Name</span></span>  <br/> |<span data-ttu-id="651c3-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="651c3-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="651c3-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="651c3-169">Validation File</span></span>  <br/> |<span data-ttu-id="651c3-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="651c3-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="651c3-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="651c3-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="651c3-172">False</span><span class="sxs-lookup"><span data-stu-id="651c3-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="651c3-173">См. также</span><span class="sxs-lookup"><span data-stu-id="651c3-173">See also</span></span>

- [<span data-ttu-id="651c3-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="651c3-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="651c3-175">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="651c3-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="651c3-176">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="651c3-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)
