---
title: Отписаться операции
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: Операция отказа от подписки используется для завершения подписку на уведомления о репликации по запросу. Используйте эту операцию, а не позволить время ожидания подписки. Эта операция допускается только для уведомления по запросу.
ms.openlocfilehash: 64514a718d473f0fd7d0320bd1ccecddb1940ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840309"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="e0749-105">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="e0749-105">Unsubscribe operation</span></span>

<span data-ttu-id="e0749-106">Операция отказа от подписки используется для завершения подписку на уведомления о репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="e0749-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="e0749-107">Используйте эту операцию, а не позволить время ожидания подписки.</span><span class="sxs-lookup"><span data-stu-id="e0749-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="e0749-108">Эта операция допускается только для уведомления по запросу.</span><span class="sxs-lookup"><span data-stu-id="e0749-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="e0749-109">Пример запроса отписаться</span><span class="sxs-lookup"><span data-stu-id="e0749-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="e0749-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0749-110">Description</span></span>

<span data-ttu-id="e0749-111">В следующем примере показано сообщение SOAP XML, которое отправляется Чтобы отписаться от службы уведомлений в клиент.</span><span class="sxs-lookup"><span data-stu-id="e0749-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="e0749-112">Программа</span><span class="sxs-lookup"><span data-stu-id="e0749-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="e0749-113">Отписаться элементы запроса</span><span class="sxs-lookup"><span data-stu-id="e0749-113">Unsubscribe request elements</span></span>

<span data-ttu-id="e0749-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0749-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e0749-115">Отписаться</span><span class="sxs-lookup"><span data-stu-id="e0749-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="e0749-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="e0749-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="e0749-117">Пример успешного ответа отказа от подписки</span><span class="sxs-lookup"><span data-stu-id="e0749-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="e0749-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e0749-118">Description</span></span>

<span data-ttu-id="e0749-119">В следующем примере показано успешного ответа на запрос отказа от подписки.</span><span class="sxs-lookup"><span data-stu-id="e0749-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e0749-120">Программа</span><span class="sxs-lookup"><span data-stu-id="e0749-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="e0749-121">Отписаться элементы ответа</span><span class="sxs-lookup"><span data-stu-id="e0749-121">Unsubscribe response elements</span></span>

<span data-ttu-id="e0749-122">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0749-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e0749-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e0749-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e0749-124">Отписаться</span><span class="sxs-lookup"><span data-stu-id="e0749-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="e0749-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0749-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0749-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0749-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="e0749-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0749-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="e0749-128">Пример ответа об ошибке отписаться</span><span class="sxs-lookup"><span data-stu-id="e0749-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="e0749-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e0749-129">Description</span></span>

<span data-ttu-id="e0749-130">В следующем примере возврату ошибки отказа от подписки происходит в ответ на при попытке отменить подписку, используя идентификатор подписки, который не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0749-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="e0749-131">Программа</span><span class="sxs-lookup"><span data-stu-id="e0749-131">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="e0749-132">Отписаться элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="e0749-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="e0749-133">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0749-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e0749-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e0749-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e0749-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="e0749-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="e0749-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0749-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0749-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0749-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="e0749-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="e0749-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e0749-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0749-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e0749-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e0749-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="e0749-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e0749-141">See also</span></span>

- [<span data-ttu-id="e0749-142">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="e0749-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="e0749-143">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="e0749-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="e0749-144">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="e0749-144">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

