---
title: Екпурл-SMS (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: f5e5e589-ee16-42a8-9cd4-ae3909fc869b
description: Элемент Екпурл-SMS определяет частичный URL-адрес, который можно сочетать со значением элемента Екпурл (POX) для создания URL-адреса, который можно использовать для доступа к параметрам службы коротких сообщений (SMS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: 24f475e7f2d54fa565cc90796a983c0bd842e4da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458686"
---
# <a name="ecpurl-sms-pox"></a>Екпурл-SMS (POX)

Элемент **екпурл-SMS** определяет частичный URL-адрес, который можно сочетать со значением элемента [екпурл (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к параметрам службы коротких сообщений (SMS) для пользователя с включенной поддержкой почты. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Екпурл-SMS (POX)](ecpurl-sms-pox.md)
  
```XML
<EcpUrl-sms/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет собой частичный URL-адрес, который можно сочетать со значением элемента [екпурл (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к параметрам SMS для пользователя. 
  
## <a name="remarks"></a>Примечания

Элемент **екпурл-SMS** — это необязательный дочерний элемент элемента **Protocol** . 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

