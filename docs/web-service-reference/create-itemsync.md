---
title: Создание (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Создать элемент определяет один элемент для создания в локальном хранилище клиента.
ms.openlocfilehash: 39056bcaab3577b1b729421118a45571910922fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761853"
---
# <a name="create-itemsync"></a><span data-ttu-id="b76f7-103">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b76f7-103">Create (ItemSync)</span></span>

<span data-ttu-id="b76f7-104">**Создать** элемент определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="b76f7-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
[<span data-ttu-id="b76f7-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b76f7-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="b76f7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b76f7-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="b76f7-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b76f7-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="b76f7-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="b76f7-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="b76f7-109">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b76f7-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 <span data-ttu-id="b76f7-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="b76f7-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b76f7-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b76f7-111">Attributes and elements</span></span>

<span data-ttu-id="b76f7-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b76f7-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b76f7-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b76f7-113">Attributes</span></span>

<span data-ttu-id="b76f7-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="b76f7-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b76f7-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b76f7-115">Child elements</span></span>

|<span data-ttu-id="b76f7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b76f7-116">**Element**</span></span>|<span data-ttu-id="b76f7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b76f7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b76f7-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="b76f7-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="b76f7-119">Представляет универсальный элемент Exchange для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-120">Message</span><span class="sxs-lookup"><span data-stu-id="b76f7-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b76f7-121">Представляет сообщение электронной почты Exchange для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-122">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="b76f7-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b76f7-123">Представляет элемент календаря Exchange для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="b76f7-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b76f7-125">Представляет элемент контакта Exchange для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b76f7-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b76f7-127">Представляет список рассылки, чтобы создать.</span><span class="sxs-lookup"><span data-stu-id="b76f7-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b76f7-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b76f7-129">Представляет сообщение собрания для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b76f7-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b76f7-131">Представляет Создание приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="b76f7-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b76f7-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b76f7-133">Представляет ответ на приглашение для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b76f7-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b76f7-135">Представляет отмены собрания для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="b76f7-136">Задача</span><span class="sxs-lookup"><span data-stu-id="b76f7-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="b76f7-137">Представляет задачу для создания.</span><span class="sxs-lookup"><span data-stu-id="b76f7-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b76f7-138">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b76f7-138">Parent elements</span></span>

|<span data-ttu-id="b76f7-139">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b76f7-139">**Element**</span></span>|<span data-ttu-id="b76f7-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b76f7-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b76f7-141">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="b76f7-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="b76f7-142">Содержит массив последовательности типов изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="b76f7-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b76f7-143">Замечания</span><span class="sxs-lookup"><span data-stu-id="b76f7-143">Remarks</span></span>

<span data-ttu-id="b76f7-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b76f7-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b76f7-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b76f7-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b76f7-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b76f7-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b76f7-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b76f7-147">Schema name</span></span>  <br/> |<span data-ttu-id="b76f7-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b76f7-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="b76f7-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b76f7-149">Validation file</span></span>  <br/> |<span data-ttu-id="b76f7-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b76f7-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b76f7-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b76f7-151">Can be empty</span></span>  <br/> |<span data-ttu-id="b76f7-152">False</span><span class="sxs-lookup"><span data-stu-id="b76f7-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b76f7-153">См. также</span><span class="sxs-lookup"><span data-stu-id="b76f7-153">See also</span></span>



[<span data-ttu-id="b76f7-154">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b76f7-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="b76f7-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b76f7-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

