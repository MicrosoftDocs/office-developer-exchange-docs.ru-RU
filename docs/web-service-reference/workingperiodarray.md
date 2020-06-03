---
title: воркингпериодаррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: Элемент Воркингпериодаррай содержит сведения о рабочем периоде для пользователя почтового ящика.
ms.openlocfilehash: a9ca55866a574c5208d8561fca6daf417867fef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465200"
---
# <a name="workingperiodarray"></a><span data-ttu-id="31afc-103">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="31afc-103">WorkingPeriodArray</span></span>

<span data-ttu-id="31afc-104">Элемент **воркингпериодаррай** содержит сведения о рабочем периоде для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="31afc-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="31afc-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="31afc-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="31afc-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="31afc-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="31afc-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="31afc-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="31afc-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="31afc-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="31afc-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="31afc-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="31afc-110">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="31afc-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="31afc-111">**аррайофворкингпериод**</span><span class="sxs-lookup"><span data-stu-id="31afc-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31afc-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="31afc-112">Attributes and elements</span></span>

<span data-ttu-id="31afc-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="31afc-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31afc-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="31afc-114">Attributes</span></span>

<span data-ttu-id="31afc-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="31afc-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31afc-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="31afc-116">Child elements</span></span>

|<span data-ttu-id="31afc-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31afc-117">**Element**</span></span>|<span data-ttu-id="31afc-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31afc-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31afc-119">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="31afc-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="31afc-120">Содержит рабочие недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="31afc-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31afc-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="31afc-121">Parent elements</span></span>

|<span data-ttu-id="31afc-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31afc-122">**Element**</span></span>|<span data-ttu-id="31afc-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31afc-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31afc-124">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="31afc-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="31afc-125">Представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="31afc-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="31afc-126">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="31afc-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31afc-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="31afc-127">Remarks</span></span>

<span data-ttu-id="31afc-128">Этот элемент является обязательным, если используется элемент [воркингхаурс](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="31afc-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="31afc-129">Все дочерние элементы перечислены в той последовательности, в которой они выполняются.</span><span class="sxs-lookup"><span data-stu-id="31afc-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="31afc-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="31afc-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31afc-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="31afc-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31afc-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="31afc-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31afc-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="31afc-133">Schema Name</span></span>  <br/> |<span data-ttu-id="31afc-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="31afc-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="31afc-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="31afc-135">Validation File</span></span>  <br/> |<span data-ttu-id="31afc-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="31afc-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31afc-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="31afc-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="31afc-138">False</span><span class="sxs-lookup"><span data-stu-id="31afc-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31afc-139">См. также</span><span class="sxs-lookup"><span data-stu-id="31afc-139">See also</span></span>



[<span data-ttu-id="31afc-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="31afc-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="31afc-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="31afc-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="31afc-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="31afc-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

