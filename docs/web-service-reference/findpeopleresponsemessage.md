---
title: FindPeopleResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba686738-e654-404d-ab54-83c71d030350
description: Элемент FindPeopleResponseMessage указывает сообщение ответа на запрос FindPeople.
ms.openlocfilehash: 205f20b26b5097d24de45c5a5f9681f3557a6f87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762597"
---
# <a name="findpeopleresponsemessage"></a><span data-ttu-id="8fa1c-103">FindPeopleResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8fa1c-103">FindPeopleResponseMessage</span></span>

<span data-ttu-id="8fa1c-104">Элемент **FindPeopleResponseMessage** указывает сообщение ответа на запрос **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="8fa1c-104">The **FindPeopleResponseMessage** element specifies the response message for a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <People/>
   <TotalNumberOfPeopleInView/>
</FindPeopleResponseMessage>
```

 <span data-ttu-id="8fa1c-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8fa1c-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fa1c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8fa1c-106">Attributes and elements</span></span>

<span data-ttu-id="8fa1c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8fa1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fa1c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8fa1c-108">Attributes</span></span>

<span data-ttu-id="8fa1c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8fa1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fa1c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8fa1c-110">Child elements</span></span>

<span data-ttu-id="8fa1c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [людей](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span><span class="sxs-lookup"><span data-stu-id="8fa1c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [People](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fa1c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8fa1c-112">Parent elements</span></span>

[<span data-ttu-id="8fa1c-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8fa1c-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="8fa1c-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="8fa1c-114">Remarks</span></span>

<span data-ttu-id="8fa1c-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8fa1c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8fa1c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fa1c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fa1c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8fa1c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fa1c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8fa1c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8fa1c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8fa1c-119">Schema name</span></span>  <br/> |<span data-ttu-id="8fa1c-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8fa1c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8fa1c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8fa1c-121">Validation file</span></span>  <br/> |<span data-ttu-id="8fa1c-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8fa1c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8fa1c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8fa1c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8fa1c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8fa1c-124">false</span></span>  <br/> |
   

