---
title: хомефонес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: Элемент Хомефонес указывает массив номеров домашнего телефона и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: b55d6ca752a5b00a27eb158c6a22412a9f4ecdda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460836"
---
# <a name="homephones"></a>хомефонес

Элемент **хомефонес** указывает массив номеров домашнего телефона и идентификаторы их исходных атрибутов для связанного пользователя. 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 **аррайоффоненумбераттрибутедвалуестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фоненумбераттрибутедвалуе](phonenumberattributedvalue.md) <br/> |Содержит номер телефона с одним атрибутом для пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Роль](persona.md) <br/> |Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

