---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: Элемент ReminderMessageData указывает данные в сообщении напоминание.
ms.openlocfilehash: a1d01dd24030b047bd8ad025f3e1cebed0da8e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835067"
---
# <a name="remindermessagedata"></a><span data-ttu-id="36562-103">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="36562-103">ReminderMessageData</span></span>

<span data-ttu-id="36562-104">Элемент **ReminderMessageData** указывает данные в сообщении напоминание.</span><span class="sxs-lookup"><span data-stu-id="36562-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="36562-105">**ReminderMessageDataType**</span><span class="sxs-lookup"><span data-stu-id="36562-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36562-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36562-106">Attributes and elements</span></span>

<span data-ttu-id="36562-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="36562-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36562-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36562-108">Attributes</span></span>

<span data-ttu-id="36562-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="36562-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36562-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36562-110">Child elements</span></span>

<span data-ttu-id="36562-111">[ReminderText](remindertext.md) | [расположение](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span><span class="sxs-lookup"><span data-stu-id="36562-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36562-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36562-112">Parent elements</span></span>

[<span data-ttu-id="36562-113">Message</span><span class="sxs-lookup"><span data-stu-id="36562-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="36562-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="36562-114">Remarks</span></span>

<span data-ttu-id="36562-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="36562-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="36562-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="36562-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="36562-117">Версии Exchange, начиная с номер сборки 15.00.0913.09 может включать элемент **AssociatedCalendarItemId** как дочерний элемент элемента **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="36562-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="36562-118">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36562-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36562-119">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36562-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36562-120">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36562-120">Schema Name</span></span>  <br/> |<span data-ttu-id="36562-121">Схема Types</span><span class="sxs-lookup"><span data-stu-id="36562-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="36562-122">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36562-122">Validation File</span></span>  <br/> |<span data-ttu-id="36562-123">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36562-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36562-124">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36562-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="36562-125">True</span><span class="sxs-lookup"><span data-stu-id="36562-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36562-126">См. также</span><span class="sxs-lookup"><span data-stu-id="36562-126">See also</span></span>



[<span data-ttu-id="36562-127">Message</span><span class="sxs-lookup"><span data-stu-id="36562-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="36562-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36562-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
