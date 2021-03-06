---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: Элемент CreateItem определяет запрос на создание элемента в хранилище Exchange.
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527063"
---
# <a name="createitem"></a>CreateItem

Элемент **CreateItem** определяет запрос на создание элемента в хранилище Exchange. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**креатеитемтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|Атрибут|Описание|
|:-----|:-----|
|**мессажедиспоситион** <br/> |Описывает, как будет обрабатываться элемент после его создания. Этот атрибут необходим для сообщений электронной почты. Этот атрибут применяется только к сообщениям электронной почты.  <br/> |
|**сендмитингинвитатионс** <br/> |Описывает, как обрабатываются приглашения на собрания после их создания. Этот атрибут необходим для элементов календаря.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Атрибут Мессажедиспоситион

|Значение|Описание|
|:-----|:-----|
|савеонли  <br/> |Элемент Message сохраняется в папке, указанной элементом [саведитемфолдерид](saveditemfolderid.md) . Сообщения можно отправить позже с помощью [операции SendItem](senditem-operation.md). В отклике возвращается идентификатор элемента. Идентификаторы элементов не возвращаются для всех типов элементов, кроме элементов сообщения. Это относится и к объектам Response.  <br/> |
|сендонли  <br/> |Элемент отправляется, но копия не сохраняется в папке "Отправленные". Идентификатор элемента не возвращается в ответе.<br/><br/>**Note**: функция **CreateItem** не поддерживает делегированный доступ, если используется параметр сендонли, так как Целевая папка не может быть указана с помощью этого параметра. Чтобы устранить эту операцию, необходимо создать элемент, получить идентификатор элемента и затем использовать операцию SendItem для отправки элемента.           |
|SendAndSaveCopy  <br/> |Элемент отправляется, а копия сохраняется в папке, указанной с помощью элемента [саведитемфолдерид](saveditemfolderid.md) . Идентификатор элемента не возвращается в ответе.<br/><br/>**Note**: приглашения на собрания не сохраняются в папке, определяемой свойством [саведитемфолдерид](saveditemfolderid.md) . Для календаря можно указать только расположение для сохранения элементов календаря в свойстве **саведитемфолдерид** . Вы не можете управлять местом сохранения элемента приглашения на собрание. Только связанные элементы календаря копируются и сохраняются в папку, определяемую свойством **саведитемфолдерид** .           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Атрибут Сендмитингинвитатионс

|Значение|Описание|
|:-----|:-----|
|сендтононе  <br/> |Если элемент является приглашением на собрание, он сохраняется как элемент календаря, но не отправляется.  <br/> |
|сендонлитоалл  <br/> |Приглашение на собрание отправляется всем участникам, но не сохраняется в папке "Отправленные".  <br/> |
|сендтоалландсавекопи  <br/> |Приглашение на собрание отправляется всем участникам, а копия сохраняется в папке, указанной с помощью элемента [саведитемфолдерид](saveditemfolderid.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|Элемент|Описание|
|:-----|:-----|
|[саведитемфолдерид](saveditemfolderid.md) <br/> |Указывает целевую папку, в которой можно создать новый элемент. Если для атрибута **мессажедиспоситион** задано значение сендонли, будет отправлено созданное сообщение. Сообщение не будет помещено в папку, определяемую элементом [саведитемфолдерид](saveditemfolderid.md) .  <br/> |
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определяемой элементом [саведитемфолдерид](saveditemfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [креатеитемреспонсе](createitemresponse.md)  
- [Операция CreateItem](createitem-operation.md)
- [Создание сообщений электронной почты](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Создание контактов (веб-службы Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Создание задач](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Создание встреч](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

