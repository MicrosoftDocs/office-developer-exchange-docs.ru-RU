---
title: Изменения (иерархии)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Элемент изменения содержит виртуализированный массив типы изменений, которые представляют тип различия между папками на стороне клиента и папки на компьютере, на котором выполняется Microsoft Exchange Server 2007.
ms.openlocfilehash: 15e4f9f37c5e4a4083260dcf379a49beb2260030
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761681"
---
# <a name="changes-hierarchy"></a>Изменения (иерархии)

Элемент **изменения** содержит виртуализированный массив типы изменений, которые представляют тип различия между папками на стороне клиента и папки на компьютере, на котором выполняется Microsoft Exchange Server 2007. 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[Изменения (иерархии)](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **SyncFolderHierarchyChangesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Создание (FolderSync)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[Обновление (FolderSync)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Удаление (FolderSync)](delete-foldersync.md) <br/> |Определяет одну папку для удаления в локальном хранилище клиента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Содержит состояние и результат запроса SyncFolderHierarchy.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderHierarchy](syncfolderhierarchy-operation.md)


[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
