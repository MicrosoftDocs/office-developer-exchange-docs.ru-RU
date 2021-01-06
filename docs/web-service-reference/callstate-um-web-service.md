---
title: CallState (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: Элемент CallState содержит значение, которое указывает состояние вызова.
ms.openlocfilehash: 44614c460286ff49ebc2373263c1827c6be5cc08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454612"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="189ad-103">CallState (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-103">CallState (UM web service)</span></span>

<span data-ttu-id="189ad-104">Элемент **CallState** содержит значение, которое указывает состояние вызова.</span><span class="sxs-lookup"><span data-stu-id="189ad-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="189ad-105">GetCallInfoResponse (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="189ad-106">CallState (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="189ad-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="189ad-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="189ad-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="189ad-108">Attributes and elements</span></span>

<span data-ttu-id="189ad-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="189ad-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="189ad-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="189ad-110">Attributes</span></span>

<span data-ttu-id="189ad-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="189ad-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="189ad-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="189ad-112">Child elements</span></span>

<span data-ttu-id="189ad-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="189ad-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="189ad-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="189ad-114">Parent elements</span></span>

|<span data-ttu-id="189ad-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="189ad-115">**Element**</span></span>|<span data-ttu-id="189ad-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="189ad-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="189ad-117">GetCallInfoResponse (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="189ad-118">Определяет ответ на операцию [GetCallInfo (веб-служба um).](getcallinfo-operation-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="189ad-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="189ad-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="189ad-119">Text value</span></span>

<span data-ttu-id="189ad-120">Требуется текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="189ad-120">A text value is required.</span></span> <span data-ttu-id="189ad-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="189ad-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="189ad-122">Бездействие</span><span class="sxs-lookup"><span data-stu-id="189ad-122">Idle</span></span>
    
- <span data-ttu-id="189ad-123">Connecting</span><span class="sxs-lookup"><span data-stu-id="189ad-123">Connecting</span></span>
    
- <span data-ttu-id="189ad-124">Оповещение</span><span class="sxs-lookup"><span data-stu-id="189ad-124">Alerted</span></span>
    
- <span data-ttu-id="189ad-125">Подключение</span><span class="sxs-lookup"><span data-stu-id="189ad-125">Connected</span></span>
    
- <span data-ttu-id="189ad-126">Отключено</span><span class="sxs-lookup"><span data-stu-id="189ad-126">Disconnected</span></span>
    
- <span data-ttu-id="189ad-127">Входящие</span><span class="sxs-lookup"><span data-stu-id="189ad-127">Incoming</span></span>
    
- <span data-ttu-id="189ad-128">Перенос</span><span class="sxs-lookup"><span data-stu-id="189ad-128">Transferring</span></span>
    
- <span data-ttu-id="189ad-129">Переад вперед</span><span class="sxs-lookup"><span data-stu-id="189ad-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="189ad-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="189ad-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="189ad-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="189ad-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="189ad-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="189ad-132">Schema Name</span></span>  <br/> |<span data-ttu-id="189ad-133">Сообщения</span><span class="sxs-lookup"><span data-stu-id="189ad-133">Messages</span></span>  <br/> |
|<span data-ttu-id="189ad-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="189ad-134">Validation File</span></span>  <br/> |<span data-ttu-id="189ad-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="189ad-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="189ad-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="189ad-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="189ad-137">False</span><span class="sxs-lookup"><span data-stu-id="189ad-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="189ad-138">См. также</span><span class="sxs-lookup"><span data-stu-id="189ad-138">See also</span></span>



[<span data-ttu-id="189ad-139">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="189ad-140">GetCallInfoResponse (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="189ad-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

