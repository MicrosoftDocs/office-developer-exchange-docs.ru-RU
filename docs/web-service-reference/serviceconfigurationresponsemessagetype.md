---
title: сервицеконфигуратионреспонсемессажетипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: Элемент Сервицеконфигуратионреспонсемессажетипе содержит параметры конфигурации службы.
ms.openlocfilehash: fb7841f346083017319cece4479fea8bbfb6de17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835393"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="aa70f-103">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="aa70f-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="aa70f-104">Элемент **сервицеконфигуратионреспонсемессажетипе** содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="aa70f-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="aa70f-105">**сервицеконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="aa70f-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa70f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa70f-106">Attributes and elements</span></span>

<span data-ttu-id="aa70f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aa70f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa70f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa70f-108">Attributes</span></span>

|<span data-ttu-id="aa70f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="aa70f-109">**Attribute**</span></span>|<span data-ttu-id="aa70f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa70f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa70f-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="aa70f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="aa70f-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="aa70f-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="aa70f-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="aa70f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="aa70f-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="aa70f-114">-  Success</span></span>  <br/><span data-ttu-id="aa70f-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="aa70f-115">-  Warning</span></span>  <br/><span data-ttu-id="aa70f-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="aa70f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="aa70f-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="aa70f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="aa70f-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="aa70f-118">**Value**</span></span>|<span data-ttu-id="aa70f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa70f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa70f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="aa70f-120">**Success**</span></span> <br/> |<span data-ttu-id="aa70f-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="aa70f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="aa70f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="aa70f-122">**Warning**</span></span> <br/> | <span data-ttu-id="aa70f-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="aa70f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="aa70f-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="aa70f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="aa70f-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="aa70f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="aa70f-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="aa70f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="aa70f-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa70f-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="aa70f-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="aa70f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="aa70f-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa70f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="aa70f-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="aa70f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="aa70f-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="aa70f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="aa70f-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="aa70f-132">**Error**</span></span> <br/> | <span data-ttu-id="aa70f-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="aa70f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="aa70f-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="aa70f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="aa70f-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="aa70f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="aa70f-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="aa70f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="aa70f-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="aa70f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="aa70f-138">— Недопустимый атрибут или элемент в контексте</span><span class="sxs-lookup"><span data-stu-id="aa70f-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="aa70f-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="aa70f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="aa70f-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="aa70f-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="aa70f-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="aa70f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa70f-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa70f-142">Child elements</span></span>

|<span data-ttu-id="aa70f-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa70f-143">**Element**</span></span>|<span data-ttu-id="aa70f-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa70f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa70f-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="aa70f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aa70f-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="aa70f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="aa70f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aa70f-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="aa70f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="aa70f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aa70f-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="aa70f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="aa70f-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="aa70f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="aa70f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aa70f-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="aa70f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-154">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="aa70f-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="aa70f-155">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aa70f-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-156">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aa70f-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="aa70f-157">Содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="aa70f-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="aa70f-158">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="aa70f-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="aa70f-159">Содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="aa70f-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa70f-160">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa70f-160">Parent elements</span></span>

|<span data-ttu-id="aa70f-161">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa70f-161">**Element**</span></span>|<span data-ttu-id="aa70f-162">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa70f-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa70f-163">Респонсемессажес (Аррайофсервицеконфигуратионреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="aa70f-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="aa70f-164">Содержит массив ответных сообщений конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="aa70f-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa70f-165">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aa70f-165">Text value</span></span>

<span data-ttu-id="aa70f-166">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa70f-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aa70f-167">Примечания</span><span class="sxs-lookup"><span data-stu-id="aa70f-167">Remarks</span></span>

<span data-ttu-id="aa70f-168">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa70f-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa70f-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa70f-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa70f-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa70f-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa70f-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa70f-171">Schema Name</span></span>  <br/> |<span data-ttu-id="aa70f-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="aa70f-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa70f-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa70f-173">Validation File</span></span>  <br/> |<span data-ttu-id="aa70f-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aa70f-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa70f-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa70f-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa70f-176">False</span><span class="sxs-lookup"><span data-stu-id="aa70f-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa70f-177">См. также</span><span class="sxs-lookup"><span data-stu-id="aa70f-177">See also</span></span>

- [<span data-ttu-id="aa70f-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aa70f-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

