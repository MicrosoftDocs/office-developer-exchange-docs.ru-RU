---
title: IsVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 403acdd5-3b79-46f4-9894-ba57e10085e4
description: Элемент IsVisible указывает, видима ли политика хранения для пользователей.
ms.openlocfilehash: c08b8a3d537c062d3a1a8ed59823bc0f74eea426
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834133"
---
# <a name="isvisible"></a>IsVisible

Элемент **IsVisible** указывает, видима ли политика хранения для пользователей. 
  
```XML
<IsVisible> true | false</IsVisible>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** для элемента **IsVisible** указывает, что политика хранения является видимым для пользователя. Значение **false** указывает, что политика хранения не отображается для пользователей. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
