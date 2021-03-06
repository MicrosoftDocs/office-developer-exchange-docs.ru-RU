---
title: дайофвикиндекс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: Элемент Дайофвикиндекс описывает неделю месяца, используемую в относительных шаблонах повторения.
ms.openlocfilehash: c9235d83a944f9c8883439dd2adf190b88977f16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529212"
---
# <a name="dayofweekindex"></a>дайофвикиндекс

Элемент **дайофвикиндекс** описывает неделю месяца, используемую в относительных шаблонах повторения. 
  
```xml
<DayOfWeekIndex/>
```

**дайофвикиндекстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[релативэйеарлирекурренце](relativeyearlyrecurrence.md) <br/> |Описывает относительный ежегодный шаблон повторения.  <br/> |
|[релативемонслирекурренце](relativemonthlyrecurrence.md) <br/> |Описывает относительный месячный шаблон повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже перечислены возможные значения.
  
- Первый    
- Секунды    
- Стороннего    
- 12    
- Последнее
    
## <a name="remarks"></a>Примечания

Например, второй понедельник месяца может встретиться в третьей неделе этого месяца. Если месяц начинается в пятницу, первая неделя месяца содержит только несколько дней и не содержит понедельник. Таким образом, первый понедельник должен быть в течение второй недели.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

