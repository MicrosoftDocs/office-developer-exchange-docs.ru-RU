---
title: персонаид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eec3a468-afd5-4d72-a61e-cd1964fb686c
description: Элемент Персонаид указывает идентификатор пользователя для связанного пользователя.
ms.openlocfilehash: 77668a1b32a97eef08b3316c7d4d7c8e6494c7bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834738"
---
# <a name="personaid"></a><span data-ttu-id="371f3-103">персонаид</span><span class="sxs-lookup"><span data-stu-id="371f3-103">PersonaId</span></span>

<span data-ttu-id="371f3-104">Элемент **персонаид** указывает идентификатор пользователя для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f3-104">The **PersonaId** element specifies the persona identifier for the associated persona.</span></span> 
  
```XML
<PersonaId Id="" ChangeKey=""/>
```

 <span data-ttu-id="371f3-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="371f3-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="371f3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="371f3-106">Attributes and elements</span></span>

<span data-ttu-id="371f3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="371f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="371f3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="371f3-108">Attributes</span></span>

|<span data-ttu-id="371f3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="371f3-109">**Attribute**</span></span>|<span data-ttu-id="371f3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="371f3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="371f3-111">Id</span><span class="sxs-lookup"><span data-stu-id="371f3-111">Id</span></span>  <br/> |<span data-ttu-id="371f3-112">Текстовое значение атрибута **ID** — идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f3-112">The text value of the **Id** attribute is the identifier of the persona.</span></span>  <br/> |
|<span data-ttu-id="371f3-113">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="371f3-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="371f3-114">Текстовое значение атрибута **чанжекэй** — это ключ изменения пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f3-114">The text value of the **ChangeKey** attribute is the change key of the persona.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="371f3-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="371f3-115">Child elements</span></span>

<span data-ttu-id="371f3-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="371f3-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="371f3-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="371f3-117">Parent elements</span></span>

<span data-ttu-id="371f3-118">[Пользователь](getpersona.md) | [персоны](persona.md)</span><span class="sxs-lookup"><span data-stu-id="371f3-118">[GetPersona](getpersona.md) | [Persona](persona.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="371f3-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="371f3-119">Remarks</span></span>

<span data-ttu-id="371f3-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="371f3-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="371f3-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="371f3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="371f3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="371f3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="371f3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="371f3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="371f3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="371f3-124">Schema name</span></span>  <br/> |<span data-ttu-id="371f3-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="371f3-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="371f3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="371f3-126">Validation file</span></span>  <br/> |<span data-ttu-id="371f3-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="371f3-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="371f3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="371f3-128">Can be empty</span></span>  <br/> ||
   

