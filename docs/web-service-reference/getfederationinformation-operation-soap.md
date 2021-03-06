---
title: Операция Жетфедератионинформатион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: Операция Жетфедератионинформатион предоставляет сведения о состоянии Федерации Организации, например целевом URI, используемом при запросе маркеров, предназначенных для данной организации, а также о других доменах, Объединенных в Организации.
ms.openlocfilehash: 533b2f6d282e3287f4945df56b169f5bc93ff445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455627"
---
# <a name="getfederationinformation-operation-soap"></a>Операция Жетфедератионинформатион (SOAP)

Операция **жетфедератионинформатион** предоставляет сведения о состоянии Федерации Организации, например ЦЕЛЕВом URI, используемом при запросе маркеров, предназначенных для данной организации, а также о других доменах, Объединенных в Организации. 
  
Только Федеративные организации могут предоставлять общий доступ к календарю, контактам и сообщениям внешним пользователям.
  
## <a name="getfederationinformation-request-example"></a>Пример запроса Жетфедератионинформатион

### <a name="description"></a>Description

В приведенном ниже примере запроса **жетфедератионинформатион** показан запрос сведений о Федерации пользователя. Клиент отправляет этот запрос на сервер. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [Жетфедератионинформатионрекуестмессаже (SOAP)](getfederationinformationrequestmessage-soap.md)
    
- [Запрос (SOAP)](request-soap.md)
    
- [Домен (SOAP)](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a>Пример отклика Жетфедератионинформатион

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **жетфедератионинформатион** , отправляемый сервером клиенту. 
  
### <a name="code"></a>Код

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>Элементы Response

В отклике используются следующие элементы:
  
- [Жетфедератионинформатионреспонсемессаже (SOAP)](getfederationinformationresponsemessage-soap.md)
    
- [Отклик (SOAP)](response-soap.md)
    
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [ApplicationUri (SOAP)](applicationuri-soap.md)
    
- [Домены (SOAP)](domains-soap.md)
    
- [Домен (SOAP)](domain-soap.md)
    
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

