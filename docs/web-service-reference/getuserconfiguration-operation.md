---
title: Операция GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 71d50e3c-92bd-435f-8118-b28bb85f8138
description: Операция GetUserConfiguration возвращает объект конфигурации пользователя из папки.
ms.openlocfilehash: 6c1cdf381126e54f9b9eeaed260e7c2b23b0b2a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833687"
---
# <a name="getuserconfiguration-operation"></a><span data-ttu-id="55b5f-103">Операция GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55b5f-103">GetUserConfiguration operation</span></span>

<span data-ttu-id="55b5f-104">Операция **GetUserConfiguration** возвращает объект конфигурации пользователя из папки.</span><span class="sxs-lookup"><span data-stu-id="55b5f-104">The **GetUserConfiguration** operation gets a user configuration object from a folder.</span></span> 
  
## <a name="getuserconfiguration-request-example"></a><span data-ttu-id="55b5f-105">Пример запроса GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55b5f-105">GetUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="55b5f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="55b5f-106">Description</span></span>

<span data-ttu-id="55b5f-107">В следующем примере запрос **GetUserConfiguration** показано, как для формирования запроса, чтобы получить объект конфигурации пользователя в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="55b5f-107">The following example of a **GetUserConfiguration** request shows how to form a request to get a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="55b5f-108">Программа</span><span class="sxs-lookup"><span data-stu-id="55b5f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>Dictionary</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getuserconfiguration-response-example"></a><span data-ttu-id="55b5f-109">Пример ответа GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="55b5f-109">GetUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="55b5f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55b5f-110">Description</span></span>

<span data-ttu-id="55b5f-111">В следующем примере показано успешного ответа на запрос **GetUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="55b5f-111">The following example shows a successful response to the **GetUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="55b5f-112">Программа</span><span class="sxs-lookup"><span data-stu-id="55b5f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts">
              </t:DistinguishedFolderId>
            </t:UserConfigurationName>
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="55b5f-113">См. также</span><span class="sxs-lookup"><span data-stu-id="55b5f-113">See also</span></span>



[<span data-ttu-id="55b5f-114">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="55b5f-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="55b5f-115">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="55b5f-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

