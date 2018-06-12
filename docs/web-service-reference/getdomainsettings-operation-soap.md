---
title: Операция GetDomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: Операция GetDomainSettings извлекает заданных параметров домена для пользователя. Автообнаружение возвращает домены, которые для обнаружения и требуемые настройки эти домены.
ms.openlocfilehash: 09b1d610cd415d2d9d7d0098354521ece86f5184
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762765"
---
# <a name="getdomainsettings-operation-soap"></a>Операция GetDomainSettings (SOAP)

Операция **GetDomainSettings** извлекает заданных параметров домена для пользователя. Автообнаружение возвращает домены, которые для обнаружения и требуемые настройки эти домены. 
  
## <a name="getdomainsettings-request-example"></a>Пример запроса GetDomainSettings

### <a name="description"></a>Описание

В следующем примере запрос **GetDomainSettings** показано запроса для настройки домена **ExternalEWSUrl** пользователя. Клиент отправляет запрос на сервер. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>http://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [GetDomainSettingsRequestMessage (SOAP)](getdomainsettingsrequestmessage-soap.md)
    
- [Запрос (SOAP)](request-soap.md)
    
- [Домены (SOAP)](domains-soap.md)
    
- [Домен (SOAP)](domain-soap.md)
    
- [RequestedSettings (SOAP)](requestedsettings-soap.md)
    
- [Параметр (SOAP)](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a>Пример ответа GetDomainSettings

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **GetDomainSettings** , сервер отправляет клиенту. 
  
### <a name="code"></a>Программа

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>Элементы ответа

В ответе используются следующие элементы:
  
- [GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md)
    
- [Ответ (SOAP)](response-soap.md)
    
- [Код ошибки (SOAP)](errorcode-soap.md)
    
- [Сообщение об ошибке (SOAP)](errormessage-soap.md)
    
- [DomainResponses (SOAP)](domainresponses-soap.md)
    
- [DomainResponse (SOAP)](domainresponse-soap.md)
    
- [DomainSettingErrors (SOAP)](domainsettingerrors-soap.md)
    
- [DomainSettings (SOAP)](domainsettings-soap.md)
    
- [DomainSetting (SOAP)](domainsetting-soap.md)
    
- [Имя (SOAP)](name-soap.md)
    
- [Значение (SOAP)](value-soap.md)
    
- [RedirectTarget (SOAP)](redirecttarget-soap.md)
    
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

