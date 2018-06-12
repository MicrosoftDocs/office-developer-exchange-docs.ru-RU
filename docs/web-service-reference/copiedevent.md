---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: CopiedEvent элемент представляет событие, в котором копирование элемента или папки.
ms.openlocfilehash: 89ca9fb1fd2f4187efdec0e087d840bfee197a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761832"
---
# <a name="copiedevent"></a><span data-ttu-id="17eb5-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="17eb5-103">CopiedEvent</span></span>

<span data-ttu-id="17eb5-104">**CopiedEvent** элемент представляет событие, в котором копирование элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="17eb5-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

 <span data-ttu-id="17eb5-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="17eb5-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17eb5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="17eb5-106">Attributes and elements</span></span>

<span data-ttu-id="17eb5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="17eb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17eb5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="17eb5-108">Attributes</span></span>

<span data-ttu-id="17eb5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="17eb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17eb5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="17eb5-110">Child elements</span></span>

|<span data-ttu-id="17eb5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17eb5-111">**Element**</span></span>|<span data-ttu-id="17eb5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17eb5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17eb5-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="17eb5-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="17eb5-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="17eb5-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="17eb5-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="17eb5-116">Представляет метка времени события почтового ящика копии элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="17eb5-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="17eb5-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="17eb5-118">Представляет идентификатор папки.</span><span class="sxs-lookup"><span data-stu-id="17eb5-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="17eb5-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="17eb5-120">Представляет идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="17eb5-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="17eb5-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="17eb5-122">Представляет идентификатор папки, содержащей эту копию.</span><span class="sxs-lookup"><span data-stu-id="17eb5-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="17eb5-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="17eb5-124">Представляет идентификатор папки исходной папки, перед его скопирован.</span><span class="sxs-lookup"><span data-stu-id="17eb5-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="17eb5-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="17eb5-126">Содержит уникальный идентификатор исходного элемента, прежде чем был скопирован.</span><span class="sxs-lookup"><span data-stu-id="17eb5-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="17eb5-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="17eb5-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="17eb5-128">Содержит идентификатор исходной родительской папки, элемента или папки, который скопирован.</span><span class="sxs-lookup"><span data-stu-id="17eb5-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17eb5-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="17eb5-129">Parent elements</span></span>

|<span data-ttu-id="17eb5-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17eb5-130">**Element**</span></span>|<span data-ttu-id="17eb5-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17eb5-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17eb5-132">Уведомление</span><span class="sxs-lookup"><span data-stu-id="17eb5-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="17eb5-133">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="17eb5-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="17eb5-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="17eb5-134">Remarks</span></span>

<span data-ttu-id="17eb5-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="17eb5-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17eb5-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="17eb5-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17eb5-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="17eb5-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17eb5-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="17eb5-138">Schema name</span></span>  <br/> |<span data-ttu-id="17eb5-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="17eb5-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="17eb5-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="17eb5-140">Validation file</span></span>  <br/> |<span data-ttu-id="17eb5-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="17eb5-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17eb5-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="17eb5-142">Can be empty</span></span>  <br/> |<span data-ttu-id="17eb5-143">False</span><span class="sxs-lookup"><span data-stu-id="17eb5-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17eb5-144">См. также</span><span class="sxs-lookup"><span data-stu-id="17eb5-144">See also</span></span>



[<span data-ttu-id="17eb5-145">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="17eb5-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="17eb5-146">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="17eb5-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="17eb5-147">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="17eb5-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="17eb5-148">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="17eb5-148">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="17eb5-149">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="17eb5-149">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

