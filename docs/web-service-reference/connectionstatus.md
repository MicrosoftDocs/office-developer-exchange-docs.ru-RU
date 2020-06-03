---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: Элемент ConnectionStatus предоставляет текстовое описание состояния попотоковой подписки.
ms.openlocfilehash: 928537201041950011ae06444e3c412228d252ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462719"
---
# <a name="connectionstatus"></a><span data-ttu-id="38f09-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="38f09-103">ConnectionStatus</span></span>

<span data-ttu-id="38f09-104">Элемент **ConnectionStatus** предоставляет текстовое описание состояния попотоковой подписки.</span><span class="sxs-lookup"><span data-stu-id="38f09-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="38f09-105">**коннектионстатустипе**</span><span class="sxs-lookup"><span data-stu-id="38f09-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38f09-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38f09-106">Attributes and elements</span></span>

<span data-ttu-id="38f09-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="38f09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38f09-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38f09-108">Attributes</span></span>

<span data-ttu-id="38f09-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38f09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38f09-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38f09-110">Child elements</span></span>

<span data-ttu-id="38f09-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38f09-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38f09-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38f09-112">Parent elements</span></span>

|<span data-ttu-id="38f09-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38f09-113">**Element**</span></span>|<span data-ttu-id="38f09-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38f09-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38f09-115">жетстреаминжевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="38f09-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="38f09-116">Содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="38f09-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38f09-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="38f09-117">Text value</span></span>

<span data-ttu-id="38f09-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="38f09-118">A text value is required.</span></span> <span data-ttu-id="38f09-119">Ниже приведены возможные текстовые значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="38f09-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="38f09-120">OK</span><span class="sxs-lookup"><span data-stu-id="38f09-120">OK</span></span>
    
- <span data-ttu-id="38f09-121">Закрыто</span><span class="sxs-lookup"><span data-stu-id="38f09-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="38f09-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="38f09-122">Remarks</span></span>

<span data-ttu-id="38f09-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="38f09-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38f09-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38f09-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38f09-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38f09-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38f09-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38f09-126">Schema Name</span></span>  <br/> |<span data-ttu-id="38f09-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="38f09-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38f09-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38f09-128">Validation File</span></span>  <br/> |<span data-ttu-id="38f09-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="38f09-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38f09-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38f09-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="38f09-131">False</span><span class="sxs-lookup"><span data-stu-id="38f09-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38f09-132">См. также</span><span class="sxs-lookup"><span data-stu-id="38f09-132">See also</span></span>



[<span data-ttu-id="38f09-133">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="38f09-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="38f09-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="38f09-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

