---
title: Операция ResetPIN (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: Операция ResetPIN изменяет ПИН-код (ТЕЛЕФОННОГО интерфейса пользователя пароль) на новое случайное значение.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465494"
---
# <a name="resetpin-operation-um-web-service"></a>Операция ResetPIN (веб-служба единой системы обмена сообщениями)

Операция ResetPIN изменяет ПИН-код (ТЕЛЕФОННОГО интерфейса пользователя пароль) на новое случайное значение.
  
## <a name="remarks"></a>Примечания

Операция ResetPIN создает новый ПИН-код на основе политик ПИН-кодов. Если операция выполнена успешно, в почтовый ящик пользователя отправляется сообщение электронной почты, содержащее новый ПИН-код. Если операция завершается с ошибкой, возникает исключение, содержащее сведения об ошибке.
  
## <a name="resetpin-request-example"></a>Пример запроса ResetPIN

### <a name="description"></a>Description

В приведенном ниже примере запроса ResetPIN показано, как сформировать запрос на сброс ПИН-кода для почтового ящика.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Пример успешного ответа ResetPIN

### <a name="description"></a>Description

В приведенном ниже примере ответа ResetPIN показан ответ на запрос ResetPIN.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[ResetPIN (веб-служба единой системы обмена сообщениями)](resetpin-um-web-service.md)
  
[Ресетпинреспонсе (веб-служба единой системы обмена сообщениями)](resetpinresponse-um-web-service.md)

