---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: Элемент AddDistributionGroupToImList определяет запрос на добавление списка рассылки в список мгновенных сообщений.
ms.openlocfilehash: 90a84b23678fb0740158f601967905a8847286fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460381"
---
# <a name="adddistributiongrouptoimlist"></a>AddDistributionGroupToImList

Элемент **AddDistributionGroupToImList** определяет запрос на добавление списка рассылки в список мгновенных сообщений. 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 **адддистрибутионграуптоимлисттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[SmtpAddress](smtpaddress.md)  |  [DisplayName (нонемптистрингтипе)](displayname-nonemptystringtype.md)
  
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

