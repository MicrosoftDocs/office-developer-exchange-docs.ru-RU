---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: Элемент ResponseType представляет тип получателя ответа, полученные на собрание.
ms.openlocfilehash: fcfd47cb988ee00303b2c4205cb3d058cb6599b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835200"
---
# <a name="responsetype"></a><span data-ttu-id="90604-103">ResponseType</span><span class="sxs-lookup"><span data-stu-id="90604-103">ResponseType</span></span>

<span data-ttu-id="90604-104">Элемент **ResponseType** представляет тип получателя ответа, полученные на собрание.</span><span class="sxs-lookup"><span data-stu-id="90604-104">The **ResponseType** element represents the type of recipient response that is received for a meeting.</span></span> 
  
```xml
<ResponseType/>
```

 <span data-ttu-id="90604-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="90604-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90604-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="90604-106">Attributes and elements</span></span>

<span data-ttu-id="90604-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="90604-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90604-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="90604-108">Attributes</span></span>

<span data-ttu-id="90604-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="90604-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90604-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="90604-110">Child elements</span></span>

<span data-ttu-id="90604-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="90604-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90604-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="90604-112">Parent elements</span></span>

|<span data-ttu-id="90604-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="90604-113">**Element**</span></span>|<span data-ttu-id="90604-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90604-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90604-115">Attendee</span><span class="sxs-lookup"><span data-stu-id="90604-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="90604-116">Представляет участников и ресурсы, необходимые для собрания.</span><span class="sxs-lookup"><span data-stu-id="90604-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="90604-117">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="90604-117">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="90604-118">Представляет отмены собрания в хранилище Exchange</span><span class="sxs-lookup"><span data-stu-id="90604-118">Represents a meeting cancellation in the Exchange store</span></span>  <br/> |
|[<span data-ttu-id="90604-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="90604-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="90604-120">Представляет сообщение собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="90604-120">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="90604-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="90604-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="90604-122">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="90604-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="90604-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="90604-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="90604-124">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="90604-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90604-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="90604-125">Text value</span></span>

<span data-ttu-id="90604-126">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="90604-126">A text value is required.</span></span> <span data-ttu-id="90604-127">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="90604-127">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="90604-128">Неизвестно</span><span class="sxs-lookup"><span data-stu-id="90604-128">Unknown</span></span>
    
- <span data-ttu-id="90604-129">Organizer</span><span class="sxs-lookup"><span data-stu-id="90604-129">Organizer</span></span>
    
- <span data-ttu-id="90604-130">Под вопросом</span><span class="sxs-lookup"><span data-stu-id="90604-130">Tentative</span></span>
    
- <span data-ttu-id="90604-131">Accept</span><span class="sxs-lookup"><span data-stu-id="90604-131">Accept</span></span>
    
- <span data-ttu-id="90604-132">Отклонить</span><span class="sxs-lookup"><span data-stu-id="90604-132">Decline</span></span>
    
- <span data-ttu-id="90604-133">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="90604-133">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="90604-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="90604-134">Remarks</span></span>

<span data-ttu-id="90604-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="90604-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90604-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="90604-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90604-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="90604-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90604-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="90604-138">Schema Name</span></span>  <br/> |<span data-ttu-id="90604-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="90604-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="90604-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="90604-140">Validation File</span></span>  <br/> |<span data-ttu-id="90604-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90604-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90604-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="90604-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="90604-143">False</span><span class="sxs-lookup"><span data-stu-id="90604-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90604-144">См. также</span><span class="sxs-lookup"><span data-stu-id="90604-144">See also</span></span>



- [<span data-ttu-id="90604-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="90604-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
