---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761317"
---
# <a name="mexruntime"></a><span data-ttu-id="a3a32-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="a3a32-103">mexRuntime</span></span>
  
<span data-ttu-id="a3a32-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a3a32-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="a3a32-105">Элемент **mexRuntime** содержит элементы, определяющие данные конфигурации для наблюдение за агентом и данные конфигурации для SMTP и агенты маршрутизации, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="a3a32-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="a3a32-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="a3a32-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="a3a32-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="a3a32-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="a3a32-108">**mexRuntimeType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="a3a32-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3a32-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a3a32-109">Attributes and elements</span></span>

<span data-ttu-id="a3a32-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a3a32-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3a32-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a3a32-111">Attributes</span></span>

<span data-ttu-id="a3a32-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="a3a32-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3a32-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a3a32-113">Child elements</span></span>

|<span data-ttu-id="a3a32-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3a32-114">**Element**</span></span>|<span data-ttu-id="a3a32-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3a32-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3a32-116">мониторинг</span><span class="sxs-lookup"><span data-stu-id="a3a32-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="a3a32-117">Содержит сведения о конфигурации, который определяет, как и когда транспорта отслеживает агентов, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="a3a32-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="a3a32-118">agentList</span><span class="sxs-lookup"><span data-stu-id="a3a32-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="a3a32-119">Содержит элемент [агентов](agent.md) для каждого агента, которая устанавливается.</span><span class="sxs-lookup"><span data-stu-id="a3a32-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3a32-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a3a32-120">Parent elements</span></span>

|<span data-ttu-id="a3a32-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3a32-121">**Element**</span></span>|<span data-ttu-id="a3a32-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3a32-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3a32-123">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="a3a32-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="a3a32-124">Корневой элемент для файла конфигурации агентов.</span><span class="sxs-lookup"><span data-stu-id="a3a32-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="a3a32-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a3a32-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3a32-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a3a32-126">Namespace</span></span>  <br/> |<span data-ttu-id="a3a32-127">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="a3a32-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="a3a32-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a3a32-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a3a32-129">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="a3a32-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="a3a32-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a3a32-130">Validation File</span></span>  <br/> |<span data-ttu-id="a3a32-131">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="a3a32-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="a3a32-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a3a32-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3a32-133">false</span><span class="sxs-lookup"><span data-stu-id="a3a32-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3a32-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a3a32-134">See also</span></span>

- [<span data-ttu-id="a3a32-135">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a3a32-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)
