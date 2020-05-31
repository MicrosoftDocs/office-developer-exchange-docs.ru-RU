---
title: респонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: Элемент Респонсемессаже предоставляет описательные сведения о состоянии отклика для одной сущности в запросе.
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835191"
---
# <a name="responsemessage"></a><span data-ttu-id="e772b-103">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e772b-103">ResponseMessage</span></span>

<span data-ttu-id="e772b-104">Элемент **респонсемессаже** предоставляет описательные сведения о состоянии отклика для одной сущности в запросе.</span><span class="sxs-lookup"><span data-stu-id="e772b-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="e772b-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e772b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e772b-106">Attributes and elements</span></span>

<span data-ttu-id="e772b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e772b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e772b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e772b-108">Attributes</span></span>

|<span data-ttu-id="e772b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e772b-109">**Attribute**</span></span>|<span data-ttu-id="e772b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e772b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e772b-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="e772b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e772b-112">Представляет состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="e772b-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="e772b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e772b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e772b-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e772b-114">-  Success</span></span>  <br/><span data-ttu-id="e772b-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e772b-115">-  Warning</span></span>  <br/><span data-ttu-id="e772b-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="e772b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e772b-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e772b-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="e772b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e772b-118">**Value**</span></span>|<span data-ttu-id="e772b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e772b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e772b-120">Успешно</span><span class="sxs-lookup"><span data-stu-id="e772b-120">Success</span></span>  <br/> |<span data-ttu-id="e772b-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="e772b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e772b-122">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e772b-122">Warning</span></span>  <br/> | <span data-ttu-id="e772b-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e772b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e772b-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e772b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e772b-125">Ниже приведены некоторые возможные причины появления предупреждений.</span><span class="sxs-lookup"><span data-stu-id="e772b-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="e772b-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="e772b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e772b-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e772b-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="e772b-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="e772b-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e772b-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e772b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e772b-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="e772b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e772b-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="e772b-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="e772b-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e772b-132">Error</span></span>  <br/> | <span data-ttu-id="e772b-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e772b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e772b-134">Ниже приведены некоторые возможные причины ошибок.</span><span class="sxs-lookup"><span data-stu-id="e772b-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="e772b-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="e772b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e772b-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="e772b-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e772b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e772b-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e772b-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="e772b-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e772b-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="e772b-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e772b-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="e772b-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="e772b-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e772b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e772b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e772b-142">Child elements</span></span>

|<span data-ttu-id="e772b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e772b-143">**Element**</span></span>|<span data-ttu-id="e772b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e772b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e772b-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e772b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e772b-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e772b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e772b-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e772b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e772b-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="e772b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e772b-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e772b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e772b-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="e772b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e772b-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e772b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e772b-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e772b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e772b-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e772b-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e772b-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e772b-154">Parent elements</span></span>

|<span data-ttu-id="e772b-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e772b-155">**Element**</span></span>|<span data-ttu-id="e772b-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e772b-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e772b-157">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e772b-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="e772b-158">Содержит сведения о доступности для одного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e772b-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="e772b-159">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e772b-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="e772b-160">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e772b-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="e772b-161">Содержит данные ответа и предложения для запрошенных предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="e772b-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="e772b-162">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e772b-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="e772b-163">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e772b-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="e772b-164">Содержит результаты ответа и параметры отсутствия на отсутствие для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e772b-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="e772b-165">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e772b-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="e772b-166">сетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e772b-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="e772b-167">Содержит результат предпринятого сообщения [сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e772b-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="e772b-168">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e772b-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e772b-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="e772b-169">Remarks</span></span>

<span data-ttu-id="e772b-170">Тип **респонсемессажетипе** является общим для всех ответов на веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e772b-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="e772b-171">Тип **респонсемессажетипе** расширяется следующими сложными типами:</span><span class="sxs-lookup"><span data-stu-id="e772b-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="e772b-172">**аппликонверсатионактионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-173">**аттачментинфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-174">**делетеаттачментреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-175">**делетеитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-176">**експанддлреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-177">**финдфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-178">**финдитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-179">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-180">**жетевентсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-181">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-182">**ресолвенамесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-183">**субскрибереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-184">**сенднотификатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-185">**синкфолдерхиерарчиреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="e772b-186">**синкфолдеритемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e772b-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="e772b-187">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e772b-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="e772b-188">Различия версий</span><span class="sxs-lookup"><span data-stu-id="e772b-188">Version differences</span></span>

<span data-ttu-id="e772b-189">Типы **аппликонверсатионактионреспонсемессаже** и **делетеитемреспонсемессажетипе** были представлены в Exchange Build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="e772b-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e772b-190">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e772b-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e772b-191">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e772b-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e772b-192">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e772b-192">Schema Name</span></span>  <br/> |<span data-ttu-id="e772b-193">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e772b-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e772b-194">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e772b-194">Validation File</span></span>  <br/> |<span data-ttu-id="e772b-195">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e772b-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e772b-196">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e772b-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="e772b-197">False</span><span class="sxs-lookup"><span data-stu-id="e772b-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e772b-198">См. также</span><span class="sxs-lookup"><span data-stu-id="e772b-198">See also</span></span>

- [<span data-ttu-id="e772b-199">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e772b-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e772b-200">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e772b-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="e772b-201">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e772b-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="e772b-202">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e772b-202">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

