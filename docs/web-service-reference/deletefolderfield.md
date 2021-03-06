---
title: делетефолдерфиелд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: Элемент Делетефолдерфиелд представляет операцию удаления определенного свойства из папки во время вызова операцию UpdateFolder.
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462159"
---
# <a name="deletefolderfield"></a>делетефолдерфиелд

Элемент **делетефолдерфиелд** представляет операцию удаления определенного свойства из папки во время вызова операцию UpdateFolder. 
  
- [UpdateFolder](updatefolder.md) 
- [фолдерчанжес](folderchanges.md)  
- [FolderChange](folderchange.md)  
- [Обновления (папка)](updates-folder.md) 
- [делетефолдерфиелд](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

**делетефолдерфиелдтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет отдельные элементы свойства Dictionary.  <br/> |
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Обновления (папка)](updates-folder.md) <br/> |Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.  <br/> Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateFolder](updatefolder-operation.md)

