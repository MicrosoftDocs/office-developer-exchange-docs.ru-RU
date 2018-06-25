---
title: Состояние
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: Элемент состояние содержит кодировки Base64 формы данных синхронизации, который обновляется после каждого успешного запроса. Используется для определения состояния синхронизации.
ms.openlocfilehash: 3c600dde09fd813dcfb1f6e74671ebe9004701a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840131"
---
# <a name="syncstate"></a><span data-ttu-id="2d2c2-104">Состояние</span><span class="sxs-lookup"><span data-stu-id="2d2c2-104">SyncState</span></span>

<span data-ttu-id="2d2c2-105">Элемент **состояние** содержит кодировки Base64 формы данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="2d2c2-106">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="2d2c2-107">**Строка**</span><span class="sxs-lookup"><span data-stu-id="2d2c2-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d2c2-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d2c2-108">Attributes and elements</span></span>

<span data-ttu-id="2d2c2-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d2c2-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d2c2-110">Attributes</span></span>

<span data-ttu-id="2d2c2-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d2c2-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d2c2-112">Child elements</span></span>

<span data-ttu-id="2d2c2-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d2c2-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d2c2-114">Parent elements</span></span>

|<span data-ttu-id="2d2c2-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d2c2-115">**Element**</span></span>|<span data-ttu-id="2d2c2-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d2c2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d2c2-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="2d2c2-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="2d2c2-118">Определяет запрос для синхронизации иерархии папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="2d2c2-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2d2c2-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="2d2c2-120">Содержит состояние и результат запроса SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="2d2c2-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2d2c2-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="2d2c2-122">Определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2c2-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2d2c2-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="2d2c2-124">Содержит состояние и результат запроса SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d2c2-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2d2c2-125">Text value</span></span>

<span data-ttu-id="2d2c2-126">Текстовое значение является обязательным, если используется этот элемент.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2d2c2-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="2d2c2-127">Remarks</span></span>

<span data-ttu-id="2d2c2-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2d2c2-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d2c2-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2d2c2-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d2c2-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2d2c2-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d2c2-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2d2c2-131">Schema name</span></span>  <br/> |<span data-ttu-id="2d2c2-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2d2c2-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d2c2-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2d2c2-133">Validation file</span></span>  <br/> |<span data-ttu-id="2d2c2-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2d2c2-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d2c2-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2d2c2-135">Can be empty</span></span>  <br/> |<span data-ttu-id="2d2c2-136">False</span><span class="sxs-lookup"><span data-stu-id="2d2c2-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d2c2-137">См. также</span><span class="sxs-lookup"><span data-stu-id="2d2c2-137">See also</span></span>



[<span data-ttu-id="2d2c2-138">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="2d2c2-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="2d2c2-139">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="2d2c2-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="2d2c2-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d2c2-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

