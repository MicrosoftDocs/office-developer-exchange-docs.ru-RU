---
title: CreateItem (AcceptSharingInvitation)
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
ms.assetid: 710c893a-3037-4f04-b336-aefedd36c406
description: Операция CreateItem используется для принятия приглашения на доступ к данным календаря или контактов другого пользователя.
ms.openlocfilehash: eda846b72f42fe886497b355d9cddade7c5f4044
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457517"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="112be-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="112be-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="112be-104">Операция **CreateItem** используется для принятия приглашения на доступ к данным календаря или контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="112be-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="112be-105">Пример принятия запроса на получение приглашения на совместное использование</span><span class="sxs-lookup"><span data-stu-id="112be-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="112be-106">Description</span><span class="sxs-lookup"><span data-stu-id="112be-106">Description</span></span>

<span data-ttu-id="112be-107">В приведенном ниже примере показано, как принять приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="112be-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="112be-108">Код</span><span class="sxs-lookup"><span data-stu-id="112be-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="112be-109">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="112be-109">Request elements</span></span>

<span data-ttu-id="112be-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="112be-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="112be-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="112be-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="112be-112">Items</span><span class="sxs-lookup"><span data-stu-id="112be-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="112be-113">акцептшарингинвитатион</span><span class="sxs-lookup"><span data-stu-id="112be-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="112be-114">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="112be-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="112be-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="112be-115">Comments</span></span>

<span data-ttu-id="112be-116">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="112be-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="112be-117">Пример принятия ответа для успешного предоставления приглашения совместного доступа</span><span class="sxs-lookup"><span data-stu-id="112be-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="112be-118">Description</span><span class="sxs-lookup"><span data-stu-id="112be-118">Description</span></span>

<span data-ttu-id="112be-119">В следующем примере показан успешный ответ на запрос **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="112be-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="112be-120">Код</span><span class="sxs-lookup"><span data-stu-id="112be-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="112be-121">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="112be-121">Successful response elements</span></span>

<span data-ttu-id="112be-122">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="112be-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="112be-123">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="112be-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="112be-124">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="112be-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="112be-125">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="112be-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="112be-126">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="112be-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="112be-127">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="112be-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="112be-128">Items</span><span class="sxs-lookup"><span data-stu-id="112be-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="112be-129">Пример ответа на сообщение об ошибке принятия приглашения на совместное использование</span><span class="sxs-lookup"><span data-stu-id="112be-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="112be-130">Description</span><span class="sxs-lookup"><span data-stu-id="112be-130">Description</span></span>

<span data-ttu-id="112be-131">В следующем примере показан ответ об ошибке для запроса **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="112be-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="112be-132">Ошибка вызвана попыткой принять приглашение к совместному использованию, которое не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="112be-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="112be-133">Код</span><span class="sxs-lookup"><span data-stu-id="112be-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="112be-134">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="112be-134">Error response elements</span></span>

<span data-ttu-id="112be-135">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="112be-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="112be-136">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="112be-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="112be-137">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="112be-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="112be-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="112be-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="112be-139">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="112be-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="112be-140">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="112be-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="112be-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="112be-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="112be-142">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="112be-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="112be-143">Items</span><span class="sxs-lookup"><span data-stu-id="112be-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="112be-144">См. также</span><span class="sxs-lookup"><span data-stu-id="112be-144">See also</span></span>



[<span data-ttu-id="112be-145">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="112be-145">CreateItem operation</span></span>](createitem-operation.md)

