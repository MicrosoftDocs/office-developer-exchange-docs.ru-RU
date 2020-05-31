---
title: Операция CreateItem (сообщение электронной почты)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: Операция CreateItem используется для создания сообщений электронной почты.
ms.openlocfilehash: 591209165cfbafc2d5f4036dd8fab6659523a044
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761893"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="eaf63-103">Операция CreateItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="eaf63-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="eaf63-104">Операция CreateItem используется для создания сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="eaf63-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="eaf63-105">Пример запроса CreateItem</span><span class="sxs-lookup"><span data-stu-id="eaf63-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="eaf63-106">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf63-106">Description</span></span>

<span data-ttu-id="eaf63-107">В следующем примере запроса CreateItem показано, как создать новое сообщение электронной почты, отправить сообщение и сохранить его копию в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="eaf63-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="eaf63-108">Код</span><span class="sxs-lookup"><span data-stu-id="eaf63-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="eaf63-109">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="eaf63-109">Request elements</span></span>

<span data-ttu-id="eaf63-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eaf63-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="eaf63-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="eaf63-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="eaf63-112">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="eaf63-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="eaf63-113">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="eaf63-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="eaf63-114">Сообщение</span><span class="sxs-lookup"><span data-stu-id="eaf63-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="eaf63-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="eaf63-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="eaf63-116">Тема</span><span class="sxs-lookup"><span data-stu-id="eaf63-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="eaf63-117">Основной текст</span><span class="sxs-lookup"><span data-stu-id="eaf63-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="eaf63-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="eaf63-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="eaf63-119">Mailbox</span><span class="sxs-lookup"><span data-stu-id="eaf63-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="eaf63-120">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="eaf63-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="eaf63-121">IsRead</span><span class="sxs-lookup"><span data-stu-id="eaf63-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="eaf63-122">Чтобы найти другие параметры сообщения Request операции CreateItem, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="eaf63-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eaf63-123">Начните с элемента [CreateItem](createitem.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf63-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="eaf63-124">Успешный отклик CreateItem</span><span class="sxs-lookup"><span data-stu-id="eaf63-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="eaf63-125">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf63-125">Description</span></span>

<span data-ttu-id="eaf63-126">В следующем примере показан успешный ответ на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="eaf63-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="eaf63-127">Код</span><span class="sxs-lookup"><span data-stu-id="eaf63-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="eaf63-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="eaf63-128">Successful response elements</span></span>

<span data-ttu-id="eaf63-129">В ответ включаются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eaf63-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="eaf63-130">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="eaf63-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="eaf63-131">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="eaf63-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eaf63-132">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="eaf63-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="eaf63-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="eaf63-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eaf63-134">Items</span><span class="sxs-lookup"><span data-stu-id="eaf63-134">Items</span></span>](items.md)
    
<span data-ttu-id="eaf63-135">Чтобы найти другие параметры для ответного сообщения операции CreateItem, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="eaf63-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eaf63-136">Начните с элемента [креатеитемреспонсе](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf63-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="eaf63-137">Ошибка CreateItem Response</span><span class="sxs-lookup"><span data-stu-id="eaf63-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="eaf63-138">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf63-138">Description</span></span>

<span data-ttu-id="eaf63-139">В следующем примере показан ответ об ошибке для запроса CreateItem.</span><span class="sxs-lookup"><span data-stu-id="eaf63-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="eaf63-140">Код</span><span class="sxs-lookup"><span data-stu-id="eaf63-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="eaf63-141">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="eaf63-141">Error response elements</span></span>

<span data-ttu-id="eaf63-142">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eaf63-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="eaf63-143">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="eaf63-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="eaf63-144">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="eaf63-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eaf63-145">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="eaf63-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="eaf63-146">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="eaf63-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="eaf63-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="eaf63-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eaf63-148">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="eaf63-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="eaf63-149">Items</span><span class="sxs-lookup"><span data-stu-id="eaf63-149">Items</span></span>](items.md)
    
<span data-ttu-id="eaf63-150">Чтобы найти другие варианты сообщения об ошибке при выполнении операции CreateItem, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="eaf63-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eaf63-151">Начните с элемента [креатеитемреспонсе](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf63-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="eaf63-152">См. также</span><span class="sxs-lookup"><span data-stu-id="eaf63-152">See also</span></span>



[<span data-ttu-id="eaf63-153">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="eaf63-153">CreateItem operation</span></span>](createitem-operation.md)

