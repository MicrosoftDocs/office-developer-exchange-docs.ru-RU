---
title: копифолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: Элемент Копифолдерреспонсемессаже содержит состояние и результат одного запроса операции CopyFolder.
ms.openlocfilehash: 796ec57116e4b4943ca370e45cf0abefe7782c08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458511"
---
# <a name="copyfolderresponsemessage"></a>копифолдерреспонсемессаже

Элемент **копифолдерреспонсемессаже** содержит состояние и результат одного запроса [операции CopyFolder](copyfolder-operation.md) . 
  
- [копифолдерреспонсе](copyfolderresponse.md) 
- [респонсемессажес](responsemessages.md)  
- [копифолдерреспонсемессаже](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 **фолдеринфореспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа [операции CopyFolder](copyfolder-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения:<br/><br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.<br/><br/>Ниже приведены примеры источников предупреждений.<br/><br/>— Хранилище Exchange в пакетном режиме переключается в автономный режим.  <br/>-Доменные службы Active Directory (AD DS) переключаются в автономный режим.  <br/>— Почтовые ящики перемещаются.  <br/>— База данных сообщений (MDB) переводится в автономный режим.  <br/>— Срок действия пароля истек.  <br/>— Превышена квота.  <br/> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен.<br/><br/>Ниже приведены примеры источников ошибок.  <br/><br/>— Недопустимые атрибуты или элементы  <br/>— Атрибуты или элементы выходят за пределы допустимого диапазона  <br/>— Неизвестный тег  <br/>— Атрибут или элемент не является допустимым в контексте  <br/>— Несанкционированный доступ попытался любому клиенту  <br/>Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента<br/><br/>Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для последующего использования. Он содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив скопированных папок.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CopyFolder](copyfolder-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md) 
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

