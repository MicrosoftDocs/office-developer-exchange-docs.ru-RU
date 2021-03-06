---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: Элемент UserMailbox определяет почтовый ящик пользователя.
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465319"
---
# <a name="usermailbox"></a>UserMailbox

Элемент **UserMailbox** определяет почтовый ящик пользователя. 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **усермаилбокстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Текстовое значение атрибута **ID** — идентификатор почтового ящика.  <br/> |
|IsArchive  <br/> |Текстовое значение атрибута **Archive** указывает, является ли почтовый ящик архивным. Текстовое значение **true** для атрибута **Archive** указывает на то, что почтовый ящик является архивным почтовым ящиком. Значение **false** для атрибута **Archive** указывает на то, что почтовый ящик является основным почтовым ящиком.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Почтовые ящики (аррайофусермаилбоксестипе)](mailboxes-arrayofusermailboxestype.md)  |  [Маилбоксстатистикссеарчресулт](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |true  <br/> |
   

