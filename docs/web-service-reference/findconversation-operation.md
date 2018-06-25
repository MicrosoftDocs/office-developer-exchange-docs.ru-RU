---
title: FindConversation Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 2384908a-c203-45b6-98aa-efd6a4c23aac
description: Операция FindConversation Перечисляет список бесед в папке.
ms.openlocfilehash: 7ef2167fef96a5e8441c543cac5b6800534c2eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762564"
---
# <a name="findconversation-operation"></a><span data-ttu-id="4d834-103">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="4d834-103">FindConversation operation</span></span>

<span data-ttu-id="4d834-104">Операция **FindConversation** Перечисляет список бесед в папке.</span><span class="sxs-lookup"><span data-stu-id="4d834-104">The **FindConversation** operation enumerates a list of conversations in a folder.</span></span> 
  
## <a name="findconversation-request-example"></a><span data-ttu-id="4d834-105">Пример запроса FindConversation</span><span class="sxs-lookup"><span data-stu-id="4d834-105">FindConversation request example</span></span>

### <a name="description"></a><span data-ttu-id="4d834-106">Описание</span><span class="sxs-lookup"><span data-stu-id="4d834-106">Description</span></span>

<span data-ttu-id="4d834-107">В следующем примере запрос **FindConversation** показано, как для формирования запроса для поиска первого беседы в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="4d834-107">The following example of a **FindConversation** request shows how to form a request to find the first conversation in the Inbox folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4d834-108">Программа</span><span class="sxs-lookup"><span data-stu-id="4d834-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindConversation>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="1" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id ="inbox"/>
      </m:ParentFolderId>
    </m:FindConversation>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="4d834-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="4d834-109">Request elements</span></span>

<span data-ttu-id="4d834-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4d834-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4d834-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4d834-111">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="4d834-112">FindConversation</span><span class="sxs-lookup"><span data-stu-id="4d834-112">FindConversation</span></span>](findconversation.md)
    
- [<span data-ttu-id="4d834-113">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="4d834-113">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="4d834-114">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="4d834-114">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="4d834-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="4d834-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
## <a name="successful-findconversation-response-example"></a><span data-ttu-id="4d834-116">Пример успешного ответа FindConversation</span><span class="sxs-lookup"><span data-stu-id="4d834-116">Successful FindConversation response example</span></span>

### <a name="description"></a><span data-ttu-id="4d834-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4d834-117">Description</span></span>

<span data-ttu-id="4d834-118">В следующем примере показано успешного ответа на запрос **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="4d834-118">The following example shows a successful response to a **FindConversation** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4d834-119">Программа</span><span class="sxs-lookup"><span data-stu-id="4d834-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <t:Conversation xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:ConversationId Id="AAQkADRlZDhjZDVlLzYtNDcyZi1i32hHpdc="/>
          <t:ConversationTopic>Have you heard about EWS?</t:ConversationTopic>
          <t:UniqueRecipients>
            <t:String>User1First User1Last</t:String>
          </t:UniqueRecipients>
          <t:GlobalUniqueRecipients>
            <t:String>User2First User2Last</t:String>
            <t:String>User1First User1Last</t:String>
          </t:GlobalUniqueRecipients>
          <t:UniqueSenders>
            <t:String>User2First User2Last</t:String>
          </t:UniqueSenders>
          <t:GlobalUniqueSenders>
            <t:String>User1First User1Last</t:String>
            <t:String>User2First User2Last</t:String>
          </t:GlobalUniqueSenders>
          <t:LastDeliveryTime>2010-02-09T02:20:49Z</t:LastDeliveryTime>
          <t:GlobalLastDeliveryTime>2010-02-09T02:21:01Z</t:GlobalLastDeliveryTime>
          <t:HasAttachments>false</t:HasAttachments>
          <t:GlobalHasAttachments>false</t:GlobalHasAttachments>
          <t:MessageCount>2</t:MessageCount>
          <t:GlobalMessageCount>5</t:GlobalMessageCount>
          <t:UnreadCount>0</t:UnreadCount>
          <t:Size>6474</t:Size>
          <t:GlobalSize>14497</t:GlobalSize>
          <t:ItemClasses>
            <t:ItemClass>IPM.Note</t:ItemClass>
          </t:ItemClasses>
          <t:GlobalItemClasses>
            <t:ItemClass>IPM.Note</t:ItemClass>
          </t:GlobalItemClasses>
          <t:Importance>Normal</t:Importance>
          <t:GlobalImportance>Normal</t:GlobalImportance>
          <t:ItemIds>
            <t:ItemId Id="AAMkADRlZDhjZDVlLTU3qaTQvcFtnmUZQY2FuFP93qPtAAAADXWyAAA=" ChangeKey="CQAAAA=="/>
            <t:ItemId Id="AAMkADRlZDhjZDVFtnmUZQY2vcFtnmUZQY2FuFP93qPtAAAADXWxAAA=" ChangeKey="CQAAAA=="/>
          </t:ItemIds>
          <t:GlobalItemIds>
            <t:ItemId Id="AAMkADRlZDhCQvcFtnmADU5PAACQvcFtnmUZQsdfFPPtAAAADad4AAA=" ChangeKey="CQAAAA=="/>
            <t:ItemId Id="AAqaTXQvcFtnmUZQAADU5NAACQvcFmUZQY2FuFP93qPtAAAADXWyAAA=" ChangeKey="CQAAAA=="/>
            <t:ItemId Id="AAMkFtnmUZQY2FuFP93qPtAAAADU5vcFtY2FuFP93qPtAAAADad3AAA=" ChangeKey="CQAAAA=="/>
            <t:ItemId Id="AAMkLTU3YzQvcFtnmUZQY2FuFP93qPtnmU2FuFP93qPtAAAADXWxAAA=" ChangeKey="CQAAAA=="/>
            <t:ItemId Id="AAMkADlLTU3YzYtNDAAAAAB1aGnYmUZQY2FPAmUZQY2FuqPtAAd2AAA=" ChangeKey="CQAAAA=="/>
          </t:GlobalItemIds>
        </t:Conversation>
      </Conversations>
    </FindConversationResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comment"></a><span data-ttu-id="4d834-120">Комментарий</span><span class="sxs-lookup"><span data-stu-id="4d834-120">Comment</span></span>

<span data-ttu-id="4d834-121">Идентификаторы элементов и беседы в примере URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="4d834-121">The item and conversation identifiers in the example have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="4d834-122">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="4d834-122">Successful response elements</span></span>

<span data-ttu-id="4d834-123">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4d834-123">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4d834-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4d834-124">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4d834-125">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="4d834-125">FindConversationResponse</span></span>](findconversationresponse.md)
    
- [<span data-ttu-id="4d834-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d834-126">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4d834-127">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4d834-127">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
    
- [<span data-ttu-id="4d834-128">ConversationId</span><span class="sxs-lookup"><span data-stu-id="4d834-128">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="4d834-129">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="4d834-129">ConversationTopic</span></span>](conversationtopic.md)
    
- [<span data-ttu-id="4d834-130">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="4d834-130">UniqueRecipients</span></span>](uniquerecipients.md)
    
- [<span data-ttu-id="4d834-131">Строка</span><span class="sxs-lookup"><span data-stu-id="4d834-131">String</span></span>](string.md)
    
- [<span data-ttu-id="4d834-132">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="4d834-132">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
    
- [<span data-ttu-id="4d834-133">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4d834-133">UniqueSenders</span></span>](uniquesenders.md)
    
- [<span data-ttu-id="4d834-134">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="4d834-134">GlobalUniqueSenders</span></span>](globaluniquesenders.md)
    
- [<span data-ttu-id="4d834-135">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="4d834-135">LastDeliveryTime</span></span>](lastdeliverytime.md)
    
- [<span data-ttu-id="4d834-136">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="4d834-136">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md)
    
- [<span data-ttu-id="4d834-137">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="4d834-137">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="4d834-138">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="4d834-138">GlobalHasAttachments</span></span>](globalhasattachments.md)
    
- [<span data-ttu-id="4d834-139">MessageCount</span><span class="sxs-lookup"><span data-stu-id="4d834-139">MessageCount</span></span>](messagecount.md)
    
- [<span data-ttu-id="4d834-140">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="4d834-140">GlobalMessageCount</span></span>](globalmessagecount.md)
    
- [<span data-ttu-id="4d834-141">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="4d834-141">UnreadCount</span></span>](unreadcount.md)
    
- [<span data-ttu-id="4d834-142">Размер</span><span class="sxs-lookup"><span data-stu-id="4d834-142">Size</span></span>](size.md)
    
- [<span data-ttu-id="4d834-143">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="4d834-143">GlobalSize</span></span>](globalsize.md)
    
- [<span data-ttu-id="4d834-144">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="4d834-144">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md)
    
- [<span data-ttu-id="4d834-145">ItemClass</span><span class="sxs-lookup"><span data-stu-id="4d834-145">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="4d834-146">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="4d834-146">GlobalItemClasses</span></span>](globalitemclasses.md)
    
- [<span data-ttu-id="4d834-147">Важность</span><span class="sxs-lookup"><span data-stu-id="4d834-147">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="4d834-148">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="4d834-148">GlobalImportance</span></span>](globalimportance.md)
    
- [<span data-ttu-id="4d834-149">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="4d834-149">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="4d834-150">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="4d834-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="4d834-151">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="4d834-151">GlobalItemIds</span></span>](globalitemids.md)
    
## <a name="findconversation-error-response-example"></a><span data-ttu-id="4d834-152">Пример ответа об ошибке FindConversation</span><span class="sxs-lookup"><span data-stu-id="4d834-152">FindConversation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="4d834-153">Описание</span><span class="sxs-lookup"><span data-stu-id="4d834-153">Description</span></span>

<span data-ttu-id="4d834-154">В следующем примере показано ошибочный ответ на запрос **FindConversation** , которая была вызвана ошибка проверки схемы.</span><span class="sxs-lookup"><span data-stu-id="4d834-154">The following example shows an error response to the **FindConversation** request that was caused by a schema validation error.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4d834-155">Программа</span><span class="sxs-lookup"><span data-stu-id="4d834-155">Code</span></span>

```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: The 'Id' attribute is invalid - The value 'inbox1' is invalid according to its datatype 'http://schemas.microsoft.com/exchange/services/2006/types:DistinguishedFolderIdNameType' - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>14</t:LineNumber>
          <t:LinePosition>34</t:LinePosition>
          <t:Violation>The 'Id' attribute is invalid - The value 'inbox1' is invalid according to its datatype 'http://schemas.microsoft.com/exchange/services/2006/types:DistinguishedFolderIdNameType' - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="4d834-156">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="4d834-156">Error response elements</span></span>

<span data-ttu-id="4d834-157">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4d834-157">The following elements are used in the error response:</span></span>
  
- <span data-ttu-id="4d834-158">faultcode</span><span class="sxs-lookup"><span data-stu-id="4d834-158">faultcode</span></span>
    
- <span data-ttu-id="4d834-159">faultstring</span><span class="sxs-lookup"><span data-stu-id="4d834-159">faultstring</span></span>
    
- <span data-ttu-id="4d834-160">Подробности</span><span class="sxs-lookup"><span data-stu-id="4d834-160">detail</span></span>
    
- [<span data-ttu-id="4d834-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d834-161">ResponseCode</span></span>](responsecode.md)
    
- <span data-ttu-id="4d834-162">Message</span><span class="sxs-lookup"><span data-stu-id="4d834-162">Message</span></span>
    
- [<span data-ttu-id="4d834-163">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4d834-163">MessageXml</span></span>](messagexml.md)
    
- <span data-ttu-id="4d834-164">LineNumber</span><span class="sxs-lookup"><span data-stu-id="4d834-164">LineNumber</span></span>
    
- <span data-ttu-id="4d834-165">LinePosition</span><span class="sxs-lookup"><span data-stu-id="4d834-165">LinePosition</span></span>
    
- <span data-ttu-id="4d834-166">Нарушение прав</span><span class="sxs-lookup"><span data-stu-id="4d834-166">Violation</span></span>
    
## <a name="see-also"></a><span data-ttu-id="4d834-167">См. также</span><span class="sxs-lookup"><span data-stu-id="4d834-167">See also</span></span>



[<span data-ttu-id="4d834-168">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4d834-168">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="4d834-169">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d834-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="4d834-170">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d834-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4d834-171">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="4d834-171">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

