---
title: жетдисковерисеарчконфигуратионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d963e6c-e94d-462b-8c44-95d55c848fb2
description: Элемент Жетдисковерисеарчконфигуратионреспонсе указывает ответ на запрос GetDiscoverySearchConfiguration.
ms.openlocfilehash: 98393943434b5e3460485b7d75c2b5285983f597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460983"
---
# <a name="getdiscoverysearchconfigurationresponse"></a><span data-ttu-id="48253-103">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="48253-103">GetDiscoverySearchConfigurationResponse</span></span>

<span data-ttu-id="48253-104">Элемент **жетдисковерисеарчконфигуратионреспонсе** указывает ответ на запрос **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="48253-104">The **GetDiscoverySearchConfigurationResponse** element specifies the response to a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 <span data-ttu-id="48253-105">**жетдисковерисеарчконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="48253-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48253-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="48253-106">Attributes and elements</span></span>

<span data-ttu-id="48253-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="48253-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48253-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="48253-108">Attributes</span></span>

<span data-ttu-id="48253-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="48253-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48253-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="48253-110">Child elements</span></span>

<span data-ttu-id="48253-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="48253-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48253-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="48253-112">Parent elements</span></span>

[<span data-ttu-id="48253-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="48253-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="48253-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="48253-114">Remarks</span></span>

<span data-ttu-id="48253-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="48253-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="48253-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="48253-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48253-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="48253-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48253-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="48253-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48253-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="48253-119">Schema name</span></span>  <br/> |<span data-ttu-id="48253-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="48253-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="48253-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="48253-121">Validation file</span></span>  <br/> |<span data-ttu-id="48253-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="48253-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48253-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="48253-123">Can be empty</span></span>  <br/> |<span data-ttu-id="48253-124">false</span><span class="sxs-lookup"><span data-stu-id="48253-124">false</span></span>  <br/> |
   

