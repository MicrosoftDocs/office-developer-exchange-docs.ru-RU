---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: Элемент GetUserRetentionPolicyTagsResponseMessage указывает сообщение ответа на запрос GetUserRetentionPolicyTags.
ms.openlocfilehash: db73cb7f1922d845c9565753ff8d4917b82b1259
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19833701"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="e6928-103">GetUserRetentionPolicyTagsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e6928-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="e6928-104">Элемент **GetUserRetentionPolicyTagsResponseMessage** указывает сообщение ответа на запрос **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="e6928-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="e6928-105">**GetUserRetentionPolicyTagsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e6928-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6928-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e6928-106">Attributes and elements</span></span>

<span data-ttu-id="e6928-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e6928-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6928-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e6928-108">Attributes</span></span>

<span data-ttu-id="e6928-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e6928-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6928-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e6928-110">Child elements</span></span>

<span data-ttu-id="e6928-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="e6928-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6928-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e6928-112">Parent elements</span></span>

[<span data-ttu-id="e6928-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e6928-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="e6928-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="e6928-114">Remarks</span></span>

<span data-ttu-id="e6928-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e6928-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e6928-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6928-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6928-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e6928-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6928-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e6928-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e6928-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e6928-119">Schema name</span></span>  <br/> |<span data-ttu-id="e6928-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e6928-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e6928-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e6928-121">Validation file</span></span>  <br/> |<span data-ttu-id="e6928-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e6928-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6928-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e6928-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e6928-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e6928-124">false</span></span>  <br/> |
   

