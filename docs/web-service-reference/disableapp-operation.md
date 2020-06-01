---
title: Операция DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: Поиск сведений о DisableAppной операции EWS.
ms.openlocfilehash: 8e1f3a257a70c042a01ed70da97cfa0573a2d454
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462068"
---
# <a name="disableapp-operation"></a><span data-ttu-id="b94e7-103">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-103">DisableApp operation</span></span>

<span data-ttu-id="b94e7-104">Поиск сведений о **DisableAppной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="b94e7-104">Find information about the **DisableApp** EWS operation.</span></span> 
  
<span data-ttu-id="b94e7-105">Операция **DisableApp** отключает почтовое приложение для Outlook.</span><span class="sxs-lookup"><span data-stu-id="b94e7-105">The **DisableApp** operation disables a mail app for Outlook.</span></span> 
  
<span data-ttu-id="b94e7-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b94e7-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-disableapp-operation"></a><span data-ttu-id="b94e7-107">Использование операции DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-107">Using the DisableApp operation</span></span>

<span data-ttu-id="b94e7-108">Операция **DisableApp** принимает в запросе два аргумента, которые определяют, что почтовое приложение будет отключено, и причины, по которым оно было отключено.</span><span class="sxs-lookup"><span data-stu-id="b94e7-108">The **DisableApp** operation takes two arguments in the request that identify the mail app to disable and the reason why it was disabled.</span></span> 
  
### <a name="disableapp-operation-soap-headers"></a><span data-ttu-id="b94e7-109">Заголовки SOAP операции DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-109">DisableApp operation SOAP headers</span></span>

<span data-ttu-id="b94e7-110">Операция **DisableApp** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="b94e7-110">The **DisableApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b94e7-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="b94e7-111">**Header name**</span></span>|<span data-ttu-id="b94e7-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b94e7-112">**Element**</span></span>|<span data-ttu-id="b94e7-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b94e7-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b94e7-114">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="b94e7-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b94e7-115">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="b94e7-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b94e7-116">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="b94e7-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b94e7-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="b94e7-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b94e7-118">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="b94e7-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b94e7-119">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="b94e7-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b94e7-120">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="b94e7-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b94e7-121">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="b94e7-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a><span data-ttu-id="b94e7-122">Пример запроса операции DisableApp: Отключение почтового приложения, установленного в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="b94e7-122">DisableApp operation request example: Disable a mail app installed in a mailbox</span></span>

<span data-ttu-id="b94e7-123">В следующем примере запроса операции **DisableApp** показано, как отключить почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="b94e7-123">The following example of a **DisableApp** operation request shows how to a disable a mail app.</span></span> <span data-ttu-id="b94e7-124">Идентификатор приложения можно найти в манифесте приложения, который возвращается в ответе [операции GetAppManifests](getappmanifests-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b94e7-124">The app identifier can be found in the app manifest that is returned in a [GetAppManifests operation](getappmanifests-operation.md) response.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b94e7-125">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b94e7-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b94e7-126">DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-126">DisableApp</span></span>](disableapp.md)
    
- [<span data-ttu-id="b94e7-127">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="b94e7-127">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="b94e7-128">дисаблереасон</span><span class="sxs-lookup"><span data-stu-id="b94e7-128">DisableReason</span></span>](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a><span data-ttu-id="b94e7-129">Успешный отклик операции DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-129">Successful DisableApp operation response</span></span>

<span data-ttu-id="b94e7-130">В следующем примере показан успешный ответ на запрос операции **DisableApp** для отключения почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="b94e7-130">The following example shows a successful response to a **DisableApp** operation request to disable a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="b94e7-131">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b94e7-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b94e7-132">дисаблеаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="b94e7-132">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="b94e7-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b94e7-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a><span data-ttu-id="b94e7-134">Ответ об ошибке операции DisableApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-134">DisableApp operation error response</span></span>

<span data-ttu-id="b94e7-135">В следующем примере показан ответ об ошибке для запроса операции **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="b94e7-135">The following example shows an error response to a **DisableApp** operation request.</span></span> <span data-ttu-id="b94e7-136">Это ответ на запрос на отключение почтового приложения, которое не установлено в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b94e7-136">This is a response to a request to disable a mail app that is not installed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="b94e7-137">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b94e7-137">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b94e7-138">дисаблеаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="b94e7-138">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="b94e7-139">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b94e7-139">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b94e7-140">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b94e7-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b94e7-141">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b94e7-141">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b94e7-142">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b94e7-142">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b94e7-143">См. также</span><span class="sxs-lookup"><span data-stu-id="b94e7-143">See also</span></span>

- [<span data-ttu-id="b94e7-144">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b94e7-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="b94e7-145">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-145">InstallApp operation</span></span>](installapp-operation.md)   
- [<span data-ttu-id="b94e7-146">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="b94e7-146">UninstallApp operation</span></span>](uninstallapp-operation.md)   
- [<span data-ttu-id="b94e7-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="b94e7-147">GetAppManifests</span></span>](getappmanifests.md)   
- [<span data-ttu-id="b94e7-148">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="b94e7-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)   
- [<span data-ttu-id="b94e7-149">Надстройки Outlook</span><span class="sxs-lookup"><span data-stu-id="b94e7-149">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

