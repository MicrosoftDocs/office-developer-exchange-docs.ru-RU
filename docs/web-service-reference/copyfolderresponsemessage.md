---
title: CopyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: Элемент CopyFolderResponseMessage содержит состояние и результат одного запроса CopyFolder операции.
ms.openlocfilehash: 2bb2b407e0ae6b854d214c4b9d68ac8ed65b2c7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761839"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="dda44-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dda44-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="dda44-104">Элемент **CopyFolderResponseMessage** содержит состояние и результат одного запроса [CopyFolder операции](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dda44-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="dda44-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="dda44-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="dda44-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dda44-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="dda44-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dda44-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="dda44-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dda44-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dda44-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dda44-109">Attributes and elements</span></span>

<span data-ttu-id="dda44-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dda44-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dda44-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dda44-111">Attributes</span></span>

|<span data-ttu-id="dda44-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="dda44-112">**Attribute**</span></span>|<span data-ttu-id="dda44-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dda44-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dda44-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="dda44-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="dda44-115">Описание состояния ответа [операции CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dda44-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="dda44-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="dda44-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="dda44-117">-Success</span><span class="sxs-lookup"><span data-stu-id="dda44-117">- Success</span></span>  <br/><span data-ttu-id="dda44-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="dda44-118">-  Warning</span></span>  <br/><span data-ttu-id="dda44-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="dda44-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="dda44-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dda44-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="dda44-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dda44-121">**Value**</span></span>|<span data-ttu-id="dda44-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dda44-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dda44-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="dda44-123">**Success**</span></span> <br/> |<span data-ttu-id="dda44-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="dda44-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="dda44-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="dda44-125">**Warning**</span></span> <br/> | <span data-ttu-id="dda44-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="dda44-126">Describes a request that was not processed.</span></span> <span data-ttu-id="dda44-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="dda44-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="dda44-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="dda44-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="dda44-129">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="dda44-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="dda44-130">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="dda44-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="dda44-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="dda44-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="dda44-132">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="dda44-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="dda44-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="dda44-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="dda44-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="dda44-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="dda44-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="dda44-135">**Error**</span></span> <br/> | <span data-ttu-id="dda44-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="dda44-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="dda44-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="dda44-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="dda44-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dda44-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="dda44-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="dda44-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="dda44-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="dda44-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="dda44-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="dda44-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="dda44-142">-Предпринята попытка любой клиент несанкционированного доступа</span><span class="sxs-lookup"><span data-stu-id="dda44-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="dda44-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="dda44-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="dda44-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="dda44-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dda44-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dda44-145">Child elements</span></span>

|<span data-ttu-id="dda44-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dda44-146">**Element**</span></span>|<span data-ttu-id="dda44-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dda44-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dda44-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="dda44-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dda44-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="dda44-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dda44-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dda44-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dda44-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="dda44-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="dda44-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dda44-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dda44-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="dda44-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="dda44-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="dda44-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="dda44-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dda44-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dda44-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="dda44-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="dda44-157">Папки</span><span class="sxs-lookup"><span data-stu-id="dda44-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dda44-158">Содержит массив скопированной папки.</span><span class="sxs-lookup"><span data-stu-id="dda44-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dda44-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dda44-159">Parent elements</span></span>

|<span data-ttu-id="dda44-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dda44-160">**Element**</span></span>|<span data-ttu-id="dda44-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dda44-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dda44-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dda44-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dda44-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="dda44-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dda44-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="dda44-164">Remarks</span></span>

<span data-ttu-id="dda44-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dda44-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dda44-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dda44-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dda44-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dda44-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dda44-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dda44-168">Schema name</span></span>  <br/> |<span data-ttu-id="dda44-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dda44-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dda44-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dda44-170">Validation file</span></span>  <br/> |<span data-ttu-id="dda44-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dda44-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dda44-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dda44-172">Can be empty</span></span>  <br/> |<span data-ttu-id="dda44-173">False</span><span class="sxs-lookup"><span data-stu-id="dda44-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dda44-174">См. также</span><span class="sxs-lookup"><span data-stu-id="dda44-174">See also</span></span>

- [<span data-ttu-id="dda44-175">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="dda44-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="dda44-176">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="dda44-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="dda44-177">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dda44-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
