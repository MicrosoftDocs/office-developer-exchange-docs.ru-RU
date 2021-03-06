---
title: моривентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: Элемент Моривентс указывает, есть ли в очереди больше событий для доставки клиенту.
ms.openlocfilehash: fd12dd2e2e64ce1711e553ba5eb29bd0eb64c892
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462733"
---
# <a name="moreevents"></a>моривентс

Элемент **моривентс** указывает, есть ли в очереди больше событий для доставки клиенту. 
  
```xml
<MoreEvents/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет логическое значение. Значение **true** указывает, что в очереди есть больше событий. Значение **false** указывает, что в очереди больше нет событий. Это свойство доступно только для чтения. 
  
## <a name="remarks"></a>Примечания

В случае уведомлений о получении значение **true** в этом элементе указывает клиенту, что для получения оставшихся событий будет выдаваться другой запрос Events. Предполагается, что для спецификаций клиентов требуется минимальная задержка для уведомлений о событиях, запросы-события должны продолжаться непрерывно до тех пор, пока не будет возвращено значение **false** **моривентс** . 
  
В случае push-уведомлений значение **true** для **моривентс** указывает клиенту на то, что клиенту отправляется другой запрос уведомления для доставки оставшихся событий. Как и в случае с уведомлениями об опросе, эти дальнейшие запросы будут выполняться непрерывно, пока очередь событий на сервере клиентского доступа не будет пустой. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

