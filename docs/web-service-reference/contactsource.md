---
title: контактсаурце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: Элемент Контактсаурце описывает, находится ли контакт в хранилище Exchange или доменных службах Active Directory (AD DS).
ms.openlocfilehash: 5447dedf199c5ad6b944aa33e6dca03e83a3c340
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462712"
---
# <a name="contactsource"></a><span data-ttu-id="99f94-103">контактсаурце</span><span class="sxs-lookup"><span data-stu-id="99f94-103">ContactSource</span></span>

<span data-ttu-id="99f94-104">Элемент **контактсаурце** описывает, находится ли контакт в хранилище Exchange или доменных службах Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="99f94-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="99f94-105">**контактсаурцетипе**</span><span class="sxs-lookup"><span data-stu-id="99f94-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99f94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99f94-106">Attributes and elements</span></span>

<span data-ttu-id="99f94-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="99f94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99f94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99f94-108">Attributes</span></span>

<span data-ttu-id="99f94-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="99f94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99f94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99f94-110">Child elements</span></span>

<span data-ttu-id="99f94-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="99f94-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99f94-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99f94-112">Parent elements</span></span>

|<span data-ttu-id="99f94-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99f94-113">**Element**</span></span>|<span data-ttu-id="99f94-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99f94-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99f94-115">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="99f94-115">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="99f94-116">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="99f94-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="99f94-117">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="99f94-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="99f94-118">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="99f94-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99f94-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="99f94-119">Text value</span></span>

<span data-ttu-id="99f94-120">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="99f94-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="99f94-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="99f94-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="99f94-122">Магазин</span><span class="sxs-lookup"><span data-stu-id="99f94-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="99f94-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="99f94-123">Remarks</span></span>

<span data-ttu-id="99f94-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="99f94-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99f94-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99f94-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99f94-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99f94-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99f94-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99f94-127">Schema name</span></span>  <br/> |<span data-ttu-id="99f94-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="99f94-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="99f94-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99f94-129">Validation file</span></span>  <br/> |<span data-ttu-id="99f94-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99f94-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99f94-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99f94-131">Can be empty</span></span>  <br/> |<span data-ttu-id="99f94-132">False</span><span class="sxs-lookup"><span data-stu-id="99f94-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99f94-133">См. также</span><span class="sxs-lookup"><span data-stu-id="99f94-133">See also</span></span>



- [<span data-ttu-id="99f94-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99f94-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

