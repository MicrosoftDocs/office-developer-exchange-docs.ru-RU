---
title: Выражение IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: Выражение IsEqualTo элемент представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если они равны.
ms.openlocfilehash: a7a7deed79c271be74bb2ff16dd86605d468721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834013"
---
# <a name="isequalto"></a>Выражение IsEqualTo

**Выражение IsEqualTo** элемент представляет выражение поиска, которое сравнивает свойство с постоянным значением или другим свойством и возвращает значение true, если они равны. 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

 **IsEqualToType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает свойства MAPI.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Представляет свойство или постоянное значение для использования при сравнении с другого свойства.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ограничения](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, который он содержит.  <br/> |
|[И](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска. Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.  <br/> |
|[Или](or.md) <br/> |Представляет выражение поиска, используемая для выполнения логического или на нем выражением поиска. [Или](or.md) возвращает значение true, если какие-либо из их дочерних элементов возвращало значение true. **Или** должен иметь два или несколько дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Замечания

Для выполнения сравнения строк, рекомендуется использовать элемент [Contains](contains.md) , как она предоставляет параметры для соответствия параметров, таких как case и пробела. Используйте элемент [не](not.md) в сочетании с элемент [Contains](contains.md) для отрицания результат. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
