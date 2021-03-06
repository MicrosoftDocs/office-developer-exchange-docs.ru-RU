---
title: фрактионалпажефолдервиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: Элемент Фрактионалпажефолдервиев описывает, где начинается страничное представление, и максимальное число папок, возвращаемых в запросе FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463071"
---
# <a name="fractionalpagefolderview"></a>фрактионалпажефолдервиев

Элемент **фрактионалпажефолдервиев** описывает, где начинается страничное представление, и максимальное число папок, возвращаемых в запросе [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[фрактионалпажефолдервиев](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **фрактионалпажевиевтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**максентриесретурнед** <br/> |Определяет максимальное число результатов, возвращаемых в ответе [FindFolder](findfolder.md) . Этот атрибут является необязательным.  <br/> |
|**Числител** <br/> |Представляет числитель дробного смещения от начала набора результатов. Этот атрибут является обязательным. Числитель должен быть равен или меньше знаменателя. Этот атрибут должен представлять целое значение, равное или больше 0. Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.  <br/> |
|**Подробно** <br/> |Представляет знаменатель дробного смещения от начала общего числа папок в наборе результатов. Этот атрибут является обязательным. Этот атрибут должен представлять целое значение больше единицы. Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Определяет запрос на идентификацию папок в почтовом ящике.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Примечания

Смещение страничного представления от начала набора найденных папок описывается с помощью дробной части. Дробь, которая определяется атрибутами **числительного** и **знаменателя** , описывает, где начинается страница данных. Например, если **числитель** равен четырем и **знаменателю** равен 5, то страница возвращаемой информации начинается с записи, расположенной четырьмя-пятогоями способа в наборе результатов. 
  
Если дробная дробь имеет нулевое значение, значит начало набора результатов. Если дробь имеет значение 1, то отображается конец набора результатов.
  
> [!NOTE]
> Дробь представляет начальную точку страницы, а не количество результатов, возвращаемых в наборе результатов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

