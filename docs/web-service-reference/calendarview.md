---
title: Представления календаря
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: Элемент представления календаря определяет операцию FindItem как возвращение элементов календаря в наборе, отображенные в календаре.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761659"
---
# <a name="calendarview"></a><span data-ttu-id="8b17b-103">Представления календаря</span><span class="sxs-lookup"><span data-stu-id="8b17b-103">CalendarView</span></span>

<span data-ttu-id="8b17b-104">Элемент **представления календаря** определяет [операции FindItem](finditem-operation.md) как возвращение элементов календаря в наборе, отображенные в календаре.</span><span class="sxs-lookup"><span data-stu-id="8b17b-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="8b17b-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="8b17b-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="8b17b-106">Представления календаря</span><span class="sxs-lookup"><span data-stu-id="8b17b-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="8b17b-107">**Представления календаря**</span><span class="sxs-lookup"><span data-stu-id="8b17b-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8b17b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b17b-108">Attributes and elements</span></span>

<span data-ttu-id="8b17b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b17b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b17b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b17b-110">Attributes</span></span>

|<span data-ttu-id="8b17b-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8b17b-111">**Attribute**</span></span>|<span data-ttu-id="8b17b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b17b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b17b-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="8b17b-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="8b17b-114">Описывает максимальное число результатов, возвращаемых в ответе FindItem.</span><span class="sxs-lookup"><span data-stu-id="8b17b-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="8b17b-115">**Дата начала**</span><span class="sxs-lookup"><span data-stu-id="8b17b-115">**StartDate**</span></span> <br/> |<span data-ttu-id="8b17b-116">Идентифицирует Пуск промежуток времени, запрос для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="8b17b-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="8b17b-117">Все элементы календаря, время окончания перед **StartDate** не будут получены.</span><span class="sxs-lookup"><span data-stu-id="8b17b-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="8b17b-118">Значение **StartDate** можно указать в формате по Гринвичу (UTC), как и в 2006-01-02T12:00:00Z, или в виде, когда указан смещение местного времени и часового пояса, как и в 2006-01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="8b17b-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="8b17b-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8b17b-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="8b17b-120">**Дата окончания**</span><span class="sxs-lookup"><span data-stu-id="8b17b-120">**EndDate**</span></span> <br/> |<span data-ttu-id="8b17b-121">Определяет конец промежуток времени, запрос для элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="8b17b-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="8b17b-122">Не будут возвращены все элементы календаря, имеющие время начала, не ранее **EndDate** .</span><span class="sxs-lookup"><span data-stu-id="8b17b-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="8b17b-123">Значение **EndDate** можно указать в формате UTC, что и 2006-02-02T12:00:00Z, или в виде, когда указан смещение местного времени и часового пояса, как и в 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="8b17b-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="8b17b-124">**EndDate** должно быть больше или равно **StartDate**; в противном случае возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="8b17b-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="8b17b-125">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8b17b-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8b17b-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b17b-126">Child elements</span></span>

<span data-ttu-id="8b17b-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b17b-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b17b-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b17b-128">Parent elements</span></span>

|<span data-ttu-id="8b17b-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b17b-129">**Element**</span></span>|<span data-ttu-id="8b17b-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b17b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b17b-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="8b17b-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="8b17b-132">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8b17b-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="8b17b-133">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8b17b-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b17b-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b17b-134">Remarks</span></span>

<span data-ttu-id="8b17b-135">Если в запросе FindItem указан элемент **представления календаря** , веб-службы возвращает список элементов одного календаря и вхождения повторяющихся элементов календаря в диапазон, указанный с **StartDate** и **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="8b17b-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="8b17b-136">Если элемент **представления календаря** не указан в запросе FindItem, веб-служба возвращает список элементов одного календаря и повторяющихся элементов главного календаря.</span><span class="sxs-lookup"><span data-stu-id="8b17b-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="8b17b-137">Календарь вхождения повторяющегося элемента календаря не развертываются.</span><span class="sxs-lookup"><span data-stu-id="8b17b-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="8b17b-138">Запросы представления календаря следует выполнять только используйте следующие свойства, поскольку они поддерживают более быстрых запросов календаря.</span><span class="sxs-lookup"><span data-stu-id="8b17b-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="8b17b-139">Свойства повторения больших двоичных объектов</span><span class="sxs-lookup"><span data-stu-id="8b17b-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="8b17b-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="8b17b-140">MapiStartTime</span></span>
    
- <span data-ttu-id="8b17b-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="8b17b-141">MapiEndTime</span></span>
    
- <span data-ttu-id="8b17b-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="8b17b-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="8b17b-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="8b17b-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="8b17b-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="8b17b-144">MapiSubject</span></span>
    
- <span data-ttu-id="8b17b-145">Location</span><span class="sxs-lookup"><span data-stu-id="8b17b-145">Location</span></span>
    
- <span data-ttu-id="8b17b-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="8b17b-146">AppointmentColor</span></span>
    
- <span data-ttu-id="8b17b-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="8b17b-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="8b17b-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="8b17b-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="8b17b-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="8b17b-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="8b17b-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="8b17b-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="8b17b-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="8b17b-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="8b17b-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="8b17b-152">AppointmentState</span></span>
    
- <span data-ttu-id="8b17b-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="8b17b-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="8b17b-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="8b17b-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="8b17b-155">Вычисляется из основного повторения больших двоичных объектов или образец</span><span class="sxs-lookup"><span data-stu-id="8b17b-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="8b17b-156">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="8b17b-156">ItemId</span></span>
    
- <span data-ttu-id="8b17b-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="8b17b-157">IsRecurring</span></span>
    
- <span data-ttu-id="8b17b-158">IsException</span><span class="sxs-lookup"><span data-stu-id="8b17b-158">IsException</span></span>
    
- <span data-ttu-id="8b17b-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="8b17b-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="8b17b-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="8b17b-160">MapiStartTime</span></span>
    
- <span data-ttu-id="8b17b-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="8b17b-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="8b17b-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="8b17b-162">MapiEndTime</span></span>
    
- <span data-ttu-id="8b17b-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="8b17b-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="8b17b-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="8b17b-164">CalendarItemType</span></span>
    
- <span data-ttu-id="8b17b-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="8b17b-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="8b17b-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="8b17b-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="8b17b-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="8b17b-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="8b17b-168">Свойства элемента главного календаря</span><span class="sxs-lookup"><span data-stu-id="8b17b-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="8b17b-169">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="8b17b-169">EntryId</span></span>
    
- <span data-ttu-id="8b17b-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="8b17b-170">ChangeKey</span></span>
    
- <span data-ttu-id="8b17b-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="8b17b-171">ItemClass</span></span>
    
- <span data-ttu-id="8b17b-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8b17b-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="8b17b-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="8b17b-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="8b17b-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="8b17b-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="8b17b-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="8b17b-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="8b17b-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="8b17b-176">TimeZone</span></span>
    
- <span data-ttu-id="8b17b-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="8b17b-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="8b17b-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="8b17b-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="8b17b-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="8b17b-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="8b17b-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="8b17b-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="8b17b-181">IsException</span><span class="sxs-lookup"><span data-stu-id="8b17b-181">IsException</span></span>
    
- <span data-ttu-id="8b17b-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="8b17b-182">IsRecurring</span></span>
    
- <span data-ttu-id="8b17b-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="8b17b-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="8b17b-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="8b17b-184">ContainerClass</span></span>
    
- <span data-ttu-id="8b17b-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="8b17b-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="8b17b-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="8b17b-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="8b17b-187">Categories</span><span class="sxs-lookup"><span data-stu-id="8b17b-187">Categories</span></span>
    
<span data-ttu-id="8b17b-188">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b17b-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="8b17b-189">Пример</span><span class="sxs-lookup"><span data-stu-id="8b17b-189">Example</span></span>

<span data-ttu-id="8b17b-190">В следующем примере показано FindItem запроса.</span><span class="sxs-lookup"><span data-stu-id="8b17b-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="8b17b-191">Успешный запрос возвращает ответ, который включает в себя элементы календаря, запускаемых на 2006-05-18T00:00:00-08:00 или после, так и завершенного перед 2006-05-19T00:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="8b17b-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="8b17b-192">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b17b-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b17b-193">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b17b-193">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b17b-194">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b17b-194">Schema Name</span></span>  <br/> |<span data-ttu-id="8b17b-195">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8b17b-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b17b-196">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b17b-196">Validation File</span></span>  <br/> |<span data-ttu-id="8b17b-197">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8b17b-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b17b-198">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b17b-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b17b-199">False</span><span class="sxs-lookup"><span data-stu-id="8b17b-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b17b-200">См. также</span><span class="sxs-lookup"><span data-stu-id="8b17b-200">See also</span></span>

- [<span data-ttu-id="8b17b-201">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="8b17b-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="8b17b-202">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="8b17b-202">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
