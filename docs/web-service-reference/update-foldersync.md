---
title: Update (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: Элемент обновления определяет одну папку для обновления в локальном хранилище клиента.
ms.openlocfilehash: bf49741b2478edff450f114dc1464a0528072bea
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353506"
---
# <a name="update-foldersync"></a><span data-ttu-id="5be98-103">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="5be98-103">Update (FolderSync)</span></span>

<span data-ttu-id="5be98-104">**Обновить** элемент определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="5be98-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="5be98-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="5be98-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="5be98-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5be98-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="5be98-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5be98-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="5be98-108">Changes (Hierarchy)</span><span class="sxs-lookup"><span data-stu-id="5be98-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="5be98-109">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="5be98-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

<span data-ttu-id="5be98-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="5be98-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5be98-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5be98-111">Attributes and elements</span></span>

<span data-ttu-id="5be98-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5be98-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5be98-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5be98-113">Attributes</span></span>

<span data-ttu-id="5be98-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="5be98-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5be98-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5be98-115">Child elements</span></span>

|<span data-ttu-id="5be98-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5be98-116">**Element**</span></span>|<span data-ttu-id="5be98-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5be98-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5be98-118">Folder</span><span class="sxs-lookup"><span data-stu-id="5be98-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="5be98-119">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="5be98-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="5be98-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="5be98-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="5be98-121">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="5be98-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="5be98-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="5be98-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="5be98-123">Представляет папке контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5be98-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5be98-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="5be98-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="5be98-125">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5be98-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5be98-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="5be98-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="5be98-127">Представляет задачу папки t — это thcontained в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="5be98-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5be98-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5be98-128">Parent elements</span></span>

|<span data-ttu-id="5be98-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5be98-129">**Element**</span></span>|<span data-ttu-id="5be98-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5be98-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5be98-131">Changes (Hierarchy)</span><span class="sxs-lookup"><span data-stu-id="5be98-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="5be98-132">Содержит виртуализированный массив типов изменений, которые представляют тип различия между папками на стороне клиента и папки на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="5be98-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5be98-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="5be98-133">Remarks</span></span>

<span data-ttu-id="5be98-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5be98-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5be98-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5be98-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5be98-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5be98-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5be98-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5be98-137">Schema name</span></span>  <br/> |<span data-ttu-id="5be98-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5be98-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="5be98-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5be98-139">Validation file</span></span>  <br/> |<span data-ttu-id="5be98-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5be98-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5be98-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5be98-141">Can be empty</span></span>  <br/> |<span data-ttu-id="5be98-142">False</span><span class="sxs-lookup"><span data-stu-id="5be98-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5be98-143">См. также</span><span class="sxs-lookup"><span data-stu-id="5be98-143">See also</span></span>

- [<span data-ttu-id="5be98-144">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5be98-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="5be98-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5be98-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

