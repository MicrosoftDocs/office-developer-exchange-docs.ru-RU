---
title: комплетенаме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: Элемент Комплетенаме представляет полное имя контакта.
ms.openlocfilehash: 9b5d2646ec37b41cd88d7de61573bfb4a8746cdf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527175"
---
# <a name="completename"></a>комплетенаме

Элемент **комплетенаме** представляет полное имя контакта. 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 **комплетенаметипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Title](title.md) <br/> |Представляет название контакта.  <br/> |
|[FirstName](firstname.md) <br/> |Представляет имя контакта.  <br/> |
|[MiddleName](middlename.md) <br/> |Представляет отчество контакта.  <br/> |
|[LastName](lastname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[Suffix](suffix.md) <br/> |Представляет суффикс имени контакта.  <br/> |
|[Initials](initials.md) <br/> |Представляет инициалы контакта.  <br/> |
|[FullName](fullname.md) <br/> |Представляет полное имя контакта.  <br/> |
|[Прозвищ](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетического имени японского имени.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетического транскрипции фамилии на японском языке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Свойство Комплетенаме является частью фигуры [по умолчанию](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) . В первоначальном выпуске Microsoft Exchange Server 2007 свойство Комплетенаме возвращается [операцией GetItem](getitem-operation.md), но не [операцией FindItem](finditem-operation.md). Начиная с Exchange Server 2007 с пакетом обновления 1 (SP1), [Операция FindItem](finditem-operation.md) также возвращает свойство комплетенаме с фигурой [по умолчанию](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) . Это изменение не влияет на схему. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [комплетенаметипе](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (веб-службы Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

