---
title: дистингуишедфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: Элемент Дистингуишедфолдерид определяет папки, на которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент FolderId для определения папки.
ms.openlocfilehash: be883cbca00910b24e4c45ba047803e5a5024566
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462698"
---
# <a name="distinguishedfolderid"></a>дистингуишедфолдерид

Элемент **дистингуишедфолдерид** определяет папки, на которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент [FolderId](folderid.md) для определения папки. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **дистингуишедфолдеридтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Содержит строку, определяющую папку по умолчанию. Этот атрибут является обязательным.  <br/> |
|**чанжекэй** <br/> |Содержит строку, определяющую версию папки, определяемую атрибутом **ID** . Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
#### <a name="id-attribute-values"></a>Значения атрибута ID

|**Значение**|**Описание**|
|:-----|:-----|
|calendar  <br/> |Представляет папку "Календарь".  <br/> |
|contacts  <br/> |Представляет папку "Контакты".  <br/> |
|deleteditems  <br/> |Представляет папку "Удаленные".  <br/> |
|drafts  <br/> |Представляет папку "Черновики".  <br/> |
|inbox  <br/> |Представляет папку "Входящие".  <br/> |
|Фин  <br/> |Представляет папку журнала.  <br/> |
|notes  <br/> |Представляет папку заметок.  <br/> |
|outbox  <br/> |Представляет папку "Исходящие".  <br/> |
|sentitems  <br/> |Представляет папку "Отправленные".  <br/> |
|tasks  <br/> |Представляет папку "задачи".  <br/> |
|msgfolderroot  <br/> |Представляет корневой каталог папки сообщений.  <br/> |
|root  <br/> |Представляет корневую папку почтового ящика.  <br/> |
|junkemail  <br/> |Представляет папку нежелательной почты.  <br/> |
|searchfolders  <br/> |Представляет папку "папки поиска".  <br/> |
|voicemail  <br/> |Представляет папку голосовой почты.  <br/> |
|рековераблеитемсрут  <br/> |Представляет корневую папку корзины.  <br/> |
|recoverableitemsdeletions  <br/> |Представляет папку удаления корзины.  <br/> |
|рековераблеитемсверсионс  <br/> |Представляет папку корзины.  <br/> |
|рековераблеитемспуржес  <br/> |Представляет папку очистки корзины.  <br/> |
|арчиверут  <br/> |Представляет корневую папку архива.  <br/> |
|арчивемсгфолдеррут  <br/> |Представляет корневую папку с архивными сообщениями.  <br/> |
|арчиведелетедитемс  <br/> |Представляет папку "архивировать удаленные элементы".  <br/> |
|арчивеинбокс  <br/> |Представляет папку архива "Входящие". Версия Exchange, начинающаяся с номера сборки 15.00.0913.09, включает это значение.  <br/> |
|арчиверековераблеитемсрут  <br/> |Представляет корневую папку архивных элементов для восстановления.  <br/> |
|арчиверековераблеитемсделетионс  <br/> |Представляет папку удаления архивируемых элементов для восстановления.  <br/> |
|арчиверековераблеитемсверсионс  <br/> |Представляет папку "архивы версий элементов для восстановления".  <br/> |
|арчиверековераблеитемспуржес  <br/> |Представляет папку очистки архивируемых элементов для восстановления.  <br/> |
|syncissues  <br/> |Представляет папку "ошибки синхронизации".  <br/> |
|conflicts  <br/> |Представляет папку "конфликты".  <br/> |
|localfailures  <br/> |Представляет папку "Локальные ошибки".  <br/> |
|serverfailures  <br/> |Представляет папку "ошибки сервера".  <br/> |
|реЦипиенткаче  <br/> |Представляет папку кэша получателей.  <br/> |
|куиккконтактс  <br/> |Представляет папку "Быстрые контакты".  <br/> |
|conversationhistory  <br/> |Представляет папку "Журнал бесед".  <br/> |
|админаудитлогс  <br/> |Представляет папку "журналы аудита действий администратора".  <br/> |
|тодосеарч  <br/> |Представляет папку поиска TODO.  <br/> |
|Mycontacts  <br/> |Представляет папку "Мои контакты".  <br/> |
|каталога  <br/> |Представляет папку каталога.  <br/> |
|имконтактлист  <br/> |Представляет папку списка контактов для обмена мгновенными сообщениями.  <br/> |
|пеоплеконнект  <br/> |Представляет папку "люди Connect".  <br/> |
|Избранное  <br/> |Представляет папку "Избранное".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет основной SMTP-адрес. Адреса прокси-серверов не разрешены.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[контекстфолдерид](contextfolderid.md) <br/> |Указывает папку, предназначенную для действий беседы, в которых используются папки.  <br/> |
|[дестинатионфолдерид](destinationfolderid.md) <br/> |Указывает целевую папку для действий по копированию и перемещению бесед.  <br/> |
|[ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) <br/> | Определяет папку, в которой создается новая папка или элемент.  <br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[парентфолдеридс](parentfolderids.md) <br/> |Определяет папки для поиска [операции FindItem](finditem-operation.md) и [операции FindFolder](findfolder-operation.md).  <br/> |
|[басефолдеридс](basefolderids.md) <br/> |Представляет коллекцию папок, в которых будет выполняться поиск для определения содержимого папки поиска.  <br/> |
|[фолдеридс](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений, выполняемых над одной папкой.  <br/> <br/>Ниже приведено выражение XPath для этого элемента:<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[тофолдерид](tofolderid.md) <br/> | Представляет папку назначения для скопированного или перемещенного элемента или папки.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[саведитемфолдерид](saveditemfolderid.md) <br/> | Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[синкфолдерид](syncfolderid.md) <br/> |Представляет папку, содержащую синхронизируемые элементы.  <br/> |
|[усерконфигуратионнаме](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Представляет идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Представляет идентификатор папки, в которую будут перемещены элементы электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

**Дистингуишедфолдерид** разрешается в **FolderId**. 
  
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
- [Создание папок (веб-службы Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

