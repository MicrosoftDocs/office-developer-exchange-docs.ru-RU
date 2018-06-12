---
title: EmailUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: Элемент EmailUser указывает электронной почте.
ms.openlocfilehash: e724b3996d37a42527ec1183cef9bb6b312b8c93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762324"
---
# <a name="emailuser"></a><span data-ttu-id="7c196-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="7c196-103">EmailUser</span></span>

<span data-ttu-id="7c196-104">Элемент **EmailUser** указывает электронной почте.</span><span class="sxs-lookup"><span data-stu-id="7c196-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="7c196-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="7c196-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c196-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c196-106">Attributes and elements</span></span>

<span data-ttu-id="7c196-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7c196-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c196-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c196-108">Attributes</span></span>

<span data-ttu-id="7c196-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c196-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c196-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c196-110">Child elements</span></span>

|<span data-ttu-id="7c196-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c196-111">**Element**</span></span>|<span data-ttu-id="7c196-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c196-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c196-113">Имя (строка)</span><span class="sxs-lookup"><span data-stu-id="7c196-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="7c196-114">Указывает имя уточнения поиска или ключ или имя электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c196-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="7c196-115">Идентификатор пользователя (строка)</span><span class="sxs-lookup"><span data-stu-id="7c196-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="7c196-116">Задает идентификатор пользователя для пользователя по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="7c196-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c196-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c196-117">Parent elements</span></span>

|<span data-ttu-id="7c196-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c196-118">**Element**</span></span>|<span data-ttu-id="7c196-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c196-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c196-120">Участники</span><span class="sxs-lookup"><span data-stu-id="7c196-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="7c196-121">Указывает получателей приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="7c196-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c196-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c196-122">Remarks</span></span>

<span data-ttu-id="7c196-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7c196-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c196-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c196-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c196-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c196-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c196-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c196-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c196-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c196-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7c196-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="7c196-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7c196-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c196-129">Validation File</span></span>  <br/> |<span data-ttu-id="7c196-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c196-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c196-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c196-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7c196-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7c196-132">See also</span></span>



- [<span data-ttu-id="7c196-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c196-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
