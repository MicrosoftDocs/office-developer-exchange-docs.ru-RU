---
title: дисплайнамепрефиксес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04250f8d-1b83-43ae-8d2f-e052079bf2fc
description: Элемент Дисплайнамепрефиксес указывает массив префиксов отображаемого имени и идентификаторы их исходных атрибутов для соответствующего пользователя.
ms.openlocfilehash: 09e1e974cbe84ec8c7a4848c3367f2501269b797
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530749"
---
# <a name="displaynameprefixes"></a>дисплайнамепрефиксес

Элемент **дисплайнамепрефиксес** указывает массив префиксов отображаемого имени и идентификаторы их исходных атрибутов для соответствующего пользователя. 
  
```xml
<DisplayNamePrefixes>
    <StringAttributedValue></StringAttributedValue>
</DisplayNamePrefixes>
```

 **аррайофстрингаттрибутедвалуестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[стрингаттрибутедвалуе](stringattributedvalue.md) <br/> |Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.  <br/> |
   
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

