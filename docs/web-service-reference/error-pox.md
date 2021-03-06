---
title: Ошибка (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Элемент Error содержит ответ об ошибке автообнаружения.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530651"
---
# <a name="error-pox"></a>Ошибка (POX)

Элемент **Error** содержит ответ об ошибке автообнаружения. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Ошибка (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Time  <br/> |Представляет время, когда был возвращен ответ об ошибке.  <br/> |
|Id  <br/> |Представляет хэш имени компьютера, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Содержит код ошибки для ответа на автообнаружение ошибок.  <br/> |
|[Сообщение (POX)](message-pox.md) <br/> |Содержит сообщение об ошибке для ответа на автообнаружение ошибок.  <br/> |
|[Дебугдата (POX)](debugdata-pox.md) <br/> |Содержит данные отладки для отклика автообнаружения об ошибках.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Учетная запись (POX)](account-pox.md) <br/> |Содержит ответ об ошибке автообнаружения.  <br/> |
   
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

