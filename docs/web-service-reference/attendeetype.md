---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: Элемент AttendeeType обозначает тип участника, указанного в элементе Электронной почты (EmailAddressType). Этот элемент используется в запросах, которые содержат предложения о собраниях.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761520"
---
# <a name="attendeetype"></a><span data-ttu-id="3a2d7-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="3a2d7-104">AttendeeType</span></span>

<span data-ttu-id="3a2d7-p102">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **AttendeeType** обозначает тип участника, указанного в элементе [Электронной почты (EmailAddressType)](email-emailaddresstype.md). Этот элемент используется в запросах, которые содержат предложения о собраниях.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-p102">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element. This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="3a2d7-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3a2d7-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="3a2d7-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="3a2d7-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="3a2d7-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="3a2d7-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="3a2d7-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="3a2d7-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="3a2d7-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="3a2d7-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a2d7-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a2d7-112">Attributes and elements</span></span>

<span data-ttu-id="3a2d7-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a2d7-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a2d7-114">Attributes</span></span>

<span data-ttu-id="3a2d7-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a2d7-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a2d7-116">Child elements</span></span>

<span data-ttu-id="3a2d7-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a2d7-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a2d7-118">Parent elements</span></span>

|<span data-ttu-id="3a2d7-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a2d7-119">**Element**</span></span>|<span data-ttu-id="3a2d7-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a2d7-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a2d7-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="3a2d7-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="3a2d7-122">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="3a2d7-123">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="3a2d7-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a2d7-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3a2d7-124">Text value</span></span>

<span data-ttu-id="3a2d7-p103">Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-p103">A text value is required for this element. The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="3a2d7-127">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3a2d7-127">**Value**</span></span>|<span data-ttu-id="3a2d7-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a2d7-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a2d7-129">Organizer</span><span class="sxs-lookup"><span data-stu-id="3a2d7-129">Organizer</span></span>  <br/> |<span data-ttu-id="3a2d7-130">Пользователь почтового ящика и участник, который создал элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="3a2d7-131">Required</span><span class="sxs-lookup"><span data-stu-id="3a2d7-131">Required</span></span>  <br/> |<span data-ttu-id="3a2d7-132">Пользователь почтового ящика, который входит в число обязательных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="3a2d7-133">Optional</span><span class="sxs-lookup"><span data-stu-id="3a2d7-133">Optional</span></span>  <br/> |<span data-ttu-id="3a2d7-134">Пользователь почтового ящика, который не входит в число обязательных участников собрания.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="3a2d7-135">Room</span><span class="sxs-lookup"><span data-stu-id="3a2d7-135">Room</span></span>  <br/> |<span data-ttu-id="3a2d7-136">Объект почтового ящика, который указывает на помещение для проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="3a2d7-137">Resource</span><span class="sxs-lookup"><span data-stu-id="3a2d7-137">Resource</span></span>  <br/> |<span data-ttu-id="3a2d7-138">Оборудование, которое будет использоваться во время собрания, например, телевизор или проектор.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3a2d7-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="3a2d7-139">Remarks</span></span>

<span data-ttu-id="3a2d7-p104">Этот элемент относится к обязательным дочерним элементам элемента [MailboxData](mailboxdata.md). Он упоминается в [MailboxData](mailboxdata.md) только один раз. Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-p104">This element is a required child element of the [MailboxData](mailboxdata.md) element. This element can only occur once in the [MailboxData](mailboxdata.md) element. The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3a2d7-p105">[!Примечание] Тип схемы AttendeeType используется для включения сведений об участниках в элемент календаря. Не путайте этот элемент с элементами типа схемы AttendeeType.</span><span class="sxs-lookup"><span data-stu-id="3a2d7-p105">The AttendeeType schema type is used to represent attendees to a calendar item. Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3a2d7-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a2d7-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a2d7-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a2d7-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a2d7-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a2d7-147">Schema Name</span></span>  <br/> |<span data-ttu-id="3a2d7-148">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3a2d7-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="3a2d7-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a2d7-149">Validation File</span></span>  <br/> |<span data-ttu-id="3a2d7-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3a2d7-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a2d7-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a2d7-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a2d7-152">False</span><span class="sxs-lookup"><span data-stu-id="3a2d7-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a2d7-153">См. также</span><span class="sxs-lookup"><span data-stu-id="3a2d7-153">See also</span></span>

- [<span data-ttu-id="3a2d7-154">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3a2d7-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3a2d7-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3a2d7-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="3a2d7-156">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="3a2d7-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
