---
title: Операция GetRoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomLists
api_type:
- schema
ms.assetid: 55d451f9-547f-44ac-872e-9cb220ea7b7c
description: Операция GetRoomLists получает списков комнат, доступных в организации Exchange.
ms.openlocfilehash: 139a669bfc6b7c4bc9bd9c07f9f9cf52954860c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762904"
---
# <a name="getroomlists-operation"></a><span data-ttu-id="50a22-103">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-103">GetRoomLists operation</span></span>

<span data-ttu-id="50a22-104">Операция **GetRoomLists** получает списков комнат, доступных в организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="50a22-104">The **GetRoomLists** operation gets the room lists that are available within the Exchange organization.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="50a22-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="50a22-105">SOAP Headers</span></span>

<span data-ttu-id="50a22-106">Операция **GetRoomLists** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="50a22-106">The **GetRoomLists** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="50a22-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="50a22-107">**Header**</span></span>|<span data-ttu-id="50a22-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="50a22-108">**Element**</span></span>|<span data-ttu-id="50a22-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="50a22-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="50a22-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="50a22-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="50a22-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="50a22-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="50a22-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="50a22-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="50a22-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="50a22-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="50a22-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="50a22-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="50a22-115">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="50a22-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="50a22-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="50a22-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="50a22-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="50a22-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="50a22-118">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="50a22-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="50a22-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="50a22-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="50a22-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50a22-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="50a22-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="50a22-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getroomlists-request-example"></a><span data-ttu-id="50a22-122">Пример запроса GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-122">GetRoomLists request example</span></span>

### <a name="description"></a><span data-ttu-id="50a22-123">Описание</span><span class="sxs-lookup"><span data-stu-id="50a22-123">Description</span></span>

<span data-ttu-id="50a22-124">Ниже приведен пример **GetRoomLists** запроса, которое возвращает списков комнат, доступные на сервере.</span><span class="sxs-lookup"><span data-stu-id="50a22-124">The following is an example of a **GetRoomLists** request that returns the room lists that are available on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="50a22-125">Программа</span><span class="sxs-lookup"><span data-stu-id="50a22-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="50a22-126">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="50a22-126">Request elements</span></span>

<span data-ttu-id="50a22-127">Следующий элемент используется в запросе на:</span><span class="sxs-lookup"><span data-stu-id="50a22-127">The following element is used in the request:</span></span>
  
- [<span data-ttu-id="50a22-128">GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-128">GetRoomLists</span></span>](getroomlists.md)
    
## <a name="successful-getroomlists-response-example"></a><span data-ttu-id="50a22-129">Пример успешного ответа GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-129">Successful GetRoomLists response example</span></span>

### <a name="description"></a><span data-ttu-id="50a22-130">Описание</span><span class="sxs-lookup"><span data-stu-id="50a22-130">Description</span></span>

<span data-ttu-id="50a22-131">Ниже приведен пример ответа на запрос **GetRoomLists** .</span><span class="sxs-lookup"><span data-stu-id="50a22-131">The following is an example of a response to a **GetRoomLists** request.</span></span> <span data-ttu-id="50a22-132">В этом ответа показывает один список помещений на сервере.</span><span class="sxs-lookup"><span data-stu-id="50a22-132">This response shows one room list on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="50a22-133">Программа</span><span class="sxs-lookup"><span data-stu-id="50a22-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Address xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Name>Room List</t:Name>
          <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-getroomlists-response-elements"></a><span data-ttu-id="50a22-134">Элементы ответов успешно GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-134">Successful GetRoomLists response elements</span></span>

<span data-ttu-id="50a22-135">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="50a22-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="50a22-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50a22-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="50a22-137">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="50a22-137">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="50a22-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50a22-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="50a22-139">RoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-139">RoomLists</span></span>](roomlists.md)
    
- [<span data-ttu-id="50a22-140">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="50a22-140">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="50a22-141">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="50a22-141">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="50a22-142">MailboxType</span><span class="sxs-lookup"><span data-stu-id="50a22-142">MailboxType</span></span>](mailboxtype.md)
    
### <a name="getroomlists-error-response-example"></a><span data-ttu-id="50a22-143">Пример ответа об ошибке GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-143">GetRoomLists Error response example</span></span>

#### <a name="description"></a><span data-ttu-id="50a22-144">Описание</span><span class="sxs-lookup"><span data-stu-id="50a22-144">Description</span></span>

<span data-ttu-id="50a22-145">В следующем примере показано ответ при попытке получить список помещений с сервера, для которого не определенные списки комнаты.</span><span class="sxs-lookup"><span data-stu-id="50a22-145">The following example shows the response to an attempt to get room lists from a server that does not have any room lists defined.</span></span>
  
#### <a name="code"></a><span data-ttu-id="50a22-146">Программа</span><span class="sxs-lookup"><span data-stu-id="50a22-146">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"/>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

#### <a name="getroomlists-error-response-elements"></a><span data-ttu-id="50a22-147">Ошибка GetRoomLists элементы ответа</span><span class="sxs-lookup"><span data-stu-id="50a22-147">GetRoomLists Error response elements</span></span>

<span data-ttu-id="50a22-148">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="50a22-148">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="50a22-149">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50a22-149">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="50a22-150">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="50a22-150">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="50a22-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50a22-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="50a22-152">RoomLists</span><span class="sxs-lookup"><span data-stu-id="50a22-152">RoomLists</span></span>](roomlists.md)
    
## <a name="see-also"></a><span data-ttu-id="50a22-153">См. также</span><span class="sxs-lookup"><span data-stu-id="50a22-153">See also</span></span>



[<span data-ttu-id="50a22-154">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="50a22-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="50a22-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="50a22-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
