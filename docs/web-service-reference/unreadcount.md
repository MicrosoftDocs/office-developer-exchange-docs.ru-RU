---
title: унреадкаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnreadCount
api_type:
- schema
ms.assetid: 53b22647-1453-4707-9ea0-6a8369748d56
description: Элемент Унреадкаунт содержит количество непрочитанных элементов в папке.
ms.openlocfilehash: 72e5d47eac7618408e46ad11eb19eaebf9835502
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467223"
---
# <a name="unreadcount"></a>унреадкаунт

Элемент **унреадкаунт** содержит количество непрочитанных элементов в папке. 
  
```XML
<UnreadCount/>
```

 **xs: int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Беседы (ConversationType)](conversation-conversationtype.md) <br/> |Представляет одну беседу.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[модифиедевент](modifiedevent.md) <br/> |Представляет событие, в котором изменяется элемент или папка.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет целое значение. Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

