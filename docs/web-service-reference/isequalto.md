---
title: исекуалто
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
description: Элемент Исекуалто представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и принимает значение true, если они равны.
ms.openlocfilehash: 857192443ab0520bb26ead399bc5364cc862a4fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455298"
---
# <a name="isequalto"></a>исекуалто

Элемент **исекуалто** представляет выражение поиска, которое сравнивает свойство со значением константы или другим свойством и принимает значение true, если они равны. 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsEqualTo>
```

**исекуалтотипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет отдельные элементы словаря.  <br/> |
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет свойства MAPI.  <br/> |
|[фиелдуриорконстант](fielduriorconstant.md) <br/> |Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое инвертирует логическое значение содержащегося в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять логическую операцию и операцию между двумя или более выражениями поиска. Результат операции and имеет **значение true** , если все выражения поиска, содержащиеся в элементе и, имеют **значение true**.  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическую операцию OR для содержащегося в нем выражения поиска. [Или](or.md) возвращает значение true, если любой из дочерних элементов возвращает значение true. **Или** должно иметь не менее двух дочерних элементов.  <br/> |
   
## <a name="remarks"></a>Примечания

Чтобы выполнить сравнение строк, рассмотрите возможность использования элемента [Contains](contains.md) , так как он предоставляет параметры для сопоставления параметров, таких как регистр и пробел. Используйте элемент [Not](not.md) вместе с элементом [Contains](contains.md) , чтобы инвертировать результат. 
  
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

