---
title: Операция UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: a88cbe99-7968-454d-a545-4f92c330909f
description: Операция UploadItems загружает поток элементов в почтовый ящик Exchange.
ms.openlocfilehash: 6b002d531c7011b18ae1f88adfc2923d5a51e81c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840386"
---
# <a name="uploaditems-operation"></a><span data-ttu-id="d7b42-103">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-103">UploadItems operation</span></span>

<span data-ttu-id="d7b42-104">Операция **UploadItems** загружает поток элементов в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7b42-104">The **UploadItems** operation uploads a stream of items into an Exchange mailbox.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="d7b42-105">Операция **UploadItems** ограничен полезных максимальное импорта 25 МБ данных в кодировке base64 в MicrosoftExchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d7b42-105">The **UploadItems** operation is restricted in MicrosoftExchange Server 2010 Service Pack 1 (SP1) to a maximum import payload of 25MB of base64 encoded data.</span></span> <span data-ttu-id="d7b42-106">Параметр может быть изменен в файле web.config.</span><span class="sxs-lookup"><span data-stu-id="d7b42-106">The setting can be altered in the web.config file.</span></span> 
  
## <a name="uploaditems-request-example"></a><span data-ttu-id="d7b42-107">Пример запроса UploadItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-107">UploadItems request example</span></span>

### <a name="description"></a><span data-ttu-id="d7b42-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b42-108">Description</span></span>

<span data-ttu-id="d7b42-109">В следующем примере запрос **UploadItems** показано, как загружать два элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d7b42-109">The following example of an **UploadItems** request shows how to upload two items into a mailbox.</span></span> <span data-ttu-id="d7b42-110">Первый элемент — это новый элемент.</span><span class="sxs-lookup"><span data-stu-id="d7b42-110">The first item is a new item.</span></span> <span data-ttu-id="d7b42-111">Второй элемент является обновленной версией существующего элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d7b42-111">The second item is an updated version of an existing item in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d7b42-112">Программа</span><span class="sxs-lookup"><span data-stu-id="d7b42-112">Code</span></span>

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
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAA==" ChangeKey="AQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAAcSMAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAADACYAAAAAAAsAKQAAAAMALgAAAAAAAwA2AAAAAACwhw4=
          </t:Data>
        </t:Item>
        <t:Item CreateAction="Update">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAB==" ChangeKey="AQAAAA=="/>
          <t:ItemId Id="AAMkADhhOGU0MGM7AAA=" ChangeKey="CQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAANiAAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAALACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUA
            cwB0AGkAbgBnACAALQAgAGYAcgBvAG0AIABFAFcAUwBNAEEAAABAAD
            kAgJ2chyHuygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FOSVpBVBMO
          </t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d7b42-113">Комментарии</span><span class="sxs-lookup"><span data-stu-id="d7b42-113">Comments</span></span>

<span data-ttu-id="d7b42-114">Идентификаторы и данные элементов URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="d7b42-114">Identifiers and the item data have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="d7b42-115">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="d7b42-115">Request elements</span></span>

<span data-ttu-id="d7b42-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d7b42-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d7b42-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d7b42-117">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="d7b42-118">UploadItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-118">UploadItems</span></span>](uploaditems.md)
    
- [<span data-ttu-id="d7b42-119">Элементы (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="d7b42-119">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
    
- [<span data-ttu-id="d7b42-120">Элемент (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="d7b42-120">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
    
- [<span data-ttu-id="d7b42-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d7b42-121">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="d7b42-122">Данные (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="d7b42-122">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="d7b42-123">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="d7b42-123">ItemId</span></span>](itemid.md)
    
## <a name="successful-uploaditems-response-example"></a><span data-ttu-id="d7b42-124">Пример успешного ответа UploadItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-124">Successful UploadItems response example</span></span>

### <a name="description"></a><span data-ttu-id="d7b42-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b42-125">Description</span></span>

<span data-ttu-id="d7b42-126">В следующем примере показано успешного ответа на запрос **UploadItems** .</span><span class="sxs-lookup"><span data-stu-id="d7b42-126">The following example shows a successful response to the **UploadItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d7b42-127">Программа</span><span class="sxs-lookup"><span data-stu-id="d7b42-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
                         MinorVersion="1"
                         MajorBuildNumber="164"
                         MinorBuildNumber="0"
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhUFZ/AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQm"/>
        </m:UploadItemsResponseMessage>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGZ7AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQn"/>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d7b42-128">Комментарии</span><span class="sxs-lookup"><span data-stu-id="d7b42-128">Comments</span></span>

<span data-ttu-id="d7b42-129">Идентификаторы элементов URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="d7b42-129">Item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="d7b42-130">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="d7b42-130">Response elements</span></span>

<span data-ttu-id="d7b42-131">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d7b42-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d7b42-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7b42-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d7b42-133">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d7b42-133">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="d7b42-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7b42-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d7b42-135">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7b42-135">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="d7b42-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7b42-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7b42-137">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="d7b42-137">ItemId</span></span>](itemid.md)
    
## <a name="uploaditems-error-response-example"></a><span data-ttu-id="d7b42-138">Пример ответа об ошибке UploadItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-138">UploadItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="d7b42-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b42-139">Description</span></span>

<span data-ttu-id="d7b42-140">В следующем примере показано ответа на запрос **UploadItems** , который содержит ошибки, возникающие при попытке обновить элемент, который не удается найти в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d7b42-140">The following example shows a response to the **UploadItems** request that contains an error caused by an attempt to update an item that cannot be found in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d7b42-141">Программа</span><span class="sxs-lookup"><span data-stu-id="d7b42-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="d7b42-142">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="d7b42-142">Error response elements</span></span>

<span data-ttu-id="d7b42-143">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d7b42-143">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d7b42-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7b42-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d7b42-145">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d7b42-145">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="d7b42-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7b42-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d7b42-147">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7b42-147">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="d7b42-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7b42-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d7b42-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7b42-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7b42-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7b42-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d7b42-151">См. также</span><span class="sxs-lookup"><span data-stu-id="d7b42-151">See also</span></span>



[<span data-ttu-id="d7b42-152">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="d7b42-152">ExportItems operation</span></span>](exportitems-operation.md)


[<span data-ttu-id="d7b42-153">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d7b42-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="d7b42-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d7b42-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
