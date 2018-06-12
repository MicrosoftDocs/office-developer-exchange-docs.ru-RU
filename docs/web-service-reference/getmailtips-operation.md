---
title: Операция GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: Операция GetMailTips получает сведения о советы почты для указанного почтового ящика.
ms.openlocfilehash: 15c21bef90fdc4cbc6cd65512cdc078fcdf31e60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762844"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="a3865-103">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a3865-103">GetMailTips operation</span></span>

<span data-ttu-id="a3865-104">Операция **GetMailTips** получает сведения о советы почты для указанного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a3865-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="a3865-105">Пример запроса GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a3865-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="a3865-106">Описание</span><span class="sxs-lookup"><span data-stu-id="a3865-106">Description</span></span>

<span data-ttu-id="a3865-107">Клиент создает XML-ФАЙЛ запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="a3865-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="a3865-108">Запрос определяет лицо, которое отправляет клиенту как почтовый ящик для получения почтовые подсказки и запрашиваются какие почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="a3865-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="a3865-109">В этом примере клиент запрашивает возвращаться, что все почтовые подсказки для выбранного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a3865-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="a3865-110">Программа</span><span class="sxs-lookup"><span data-stu-id="a3865-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="a3865-111">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="a3865-111">Request elements</span></span>

<span data-ttu-id="a3865-112">В запрос включаются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a3865-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="a3865-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a3865-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="a3865-114">SendingAs</span><span class="sxs-lookup"><span data-stu-id="a3865-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="a3865-115">Получатели (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="a3865-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="a3865-116">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="a3865-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="a3865-117">Пример успешного ответа GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a3865-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="a3865-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a3865-118">Description</span></span>

<span data-ttu-id="a3865-119">В следующем примере тело Simple Object Access Protocol (SOAP) показано успешного ответа на запрос **GetMailTips** .</span><span class="sxs-lookup"><span data-stu-id="a3865-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a3865-120">Программа</span><span class="sxs-lookup"><span data-stu-id="a3865-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="a3865-121">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="a3865-121">Response elements</span></span>

<span data-ttu-id="a3865-122">В ответе включены следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a3865-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="a3865-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a3865-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a3865-124">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="a3865-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="a3865-125">См. также</span><span class="sxs-lookup"><span data-stu-id="a3865-125">See also</span></span>



[<span data-ttu-id="a3865-126">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a3865-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="a3865-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a3865-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

