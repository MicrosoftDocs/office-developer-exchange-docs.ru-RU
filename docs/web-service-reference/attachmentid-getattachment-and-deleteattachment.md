---
title: Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: Элемент идентификатора вложения AttachmentId определяет одного вложения.
ms.openlocfilehash: b0355b4a387c65e97fe973a1667e6b0a517ebf7e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761511"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="b823a-103">Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="b823a-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="b823a-104">Элемент **идентификатора вложения AttachmentId** определяет одного вложения.</span><span class="sxs-lookup"><span data-stu-id="b823a-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="b823a-105">**RequestAttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="b823a-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b823a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b823a-106">Attributes and elements</span></span>

<span data-ttu-id="b823a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b823a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b823a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b823a-108">Attributes</span></span>

|<span data-ttu-id="b823a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b823a-109">**Attribute**</span></span>|<span data-ttu-id="b823a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b823a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b823a-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="b823a-111">**Id**</span></span> <br/> |<span data-ttu-id="b823a-112">Задает идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="b823a-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b823a-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b823a-113">Child elements</span></span>

<span data-ttu-id="b823a-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="b823a-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b823a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b823a-115">Parent elements</span></span>

|<span data-ttu-id="b823a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b823a-116">**Element**</span></span>|<span data-ttu-id="b823a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b823a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b823a-118">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="b823a-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="b823a-119">Содержит массив идентификаторов вложения.</span><span class="sxs-lookup"><span data-stu-id="b823a-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="b823a-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b823a-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b823a-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="b823a-121">Remarks</span></span>

<span data-ttu-id="b823a-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b823a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b823a-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b823a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b823a-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b823a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b823a-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b823a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b823a-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b823a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="b823a-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b823a-127">Validation File</span></span>  <br/> |<span data-ttu-id="b823a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b823a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b823a-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b823a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b823a-130">False</span><span class="sxs-lookup"><span data-stu-id="b823a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b823a-131">См. также</span><span class="sxs-lookup"><span data-stu-id="b823a-131">See also</span></span>

- [<span data-ttu-id="b823a-132">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="b823a-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="b823a-133">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b823a-133">GetAttachment operation</span></span>](getattachment-operation.md)

