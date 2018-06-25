---
title: Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: Операция GetCallInfo возвращает состояние исходящих вызовов, который указан с CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762707"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="09c24-103">Операция GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="09c24-104">Операция GetCallInfo возвращает состояние исходящих вызовов, который указан с [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="09c24-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="09c24-105">Пример запроса GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="09c24-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="09c24-106">Описание</span><span class="sxs-lookup"><span data-stu-id="09c24-106">Description</span></span>

<span data-ttu-id="09c24-107">В следующем примере запрос GetCallInfo показано, как для формирования запроса для получения сведений об указанном исходящих вызовов.</span><span class="sxs-lookup"><span data-stu-id="09c24-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="09c24-108">Программа</span><span class="sxs-lookup"><span data-stu-id="09c24-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="09c24-109">Пример успешного ответа GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="09c24-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="09c24-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09c24-110">Description</span></span>

<span data-ttu-id="09c24-111">В следующем примере ответа GetCallInfo показано ответ на запрос GetCallInfo.</span><span class="sxs-lookup"><span data-stu-id="09c24-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="09c24-112">Программа</span><span class="sxs-lookup"><span data-stu-id="09c24-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="09c24-113">См. также</span><span class="sxs-lookup"><span data-stu-id="09c24-113">See also</span></span>



[<span data-ttu-id="09c24-114">GetCallInfo (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="09c24-115">GetCallInfoResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="09c24-116">CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="09c24-117">CallState (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="09c24-118">EventCause (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="09c24-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

