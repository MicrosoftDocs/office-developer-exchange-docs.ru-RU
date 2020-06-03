---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: Элемент SubscriptionStatus описывает состояние принудительной подписки.
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530946"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="97999-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="97999-103">SubscriptionStatus</span></span>

<span data-ttu-id="97999-104">Элемент **SubscriptionStatus** описывает состояние принудительной подписки.</span><span class="sxs-lookup"><span data-stu-id="97999-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="97999-105">**субскриптионстатустипе**</span><span class="sxs-lookup"><span data-stu-id="97999-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97999-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97999-106">Attributes and elements</span></span>

<span data-ttu-id="97999-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97999-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97999-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97999-108">Attributes</span></span>

<span data-ttu-id="97999-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97999-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97999-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97999-110">Child elements</span></span>

<span data-ttu-id="97999-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97999-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97999-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97999-112">Parent elements</span></span>

|<span data-ttu-id="97999-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97999-113">**Element**</span></span>|<span data-ttu-id="97999-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97999-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97999-115">сенднотификатионресулт</span><span class="sxs-lookup"><span data-stu-id="97999-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="97999-116">Содержит ответ клиентского приложения на push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="97999-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97999-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="97999-117">Text value</span></span>

<span data-ttu-id="97999-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="97999-118">A text value is required.</span></span> <span data-ttu-id="97999-119">Ниже приведены возможные текстовые значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="97999-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="97999-120">OK</span><span class="sxs-lookup"><span data-stu-id="97999-120">OK</span></span>
    
- <span data-ttu-id="97999-121">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="97999-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="97999-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="97999-122">Remarks</span></span>

<span data-ttu-id="97999-123">Этот элемент описывает состояние подписки.</span><span class="sxs-lookup"><span data-stu-id="97999-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="97999-124">Клиентское приложение принудительной подписки отправляет состояние на компьютер, на котором выполняется Exchange 2007, на котором установлена роль сервера клиентского доступа после каждого push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="97999-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="97999-125">Если значение **SubscriptionStatus** равно **Unsubscribe**, сервер клиентского доступа прекратит отправку уведомлений и завершит подписку.</span><span class="sxs-lookup"><span data-stu-id="97999-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="97999-126">Если значение **SubscriptionStatus** равно **ОК**, сервер клиентского доступа продолжит отправлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="97999-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="97999-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="97999-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97999-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97999-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97999-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97999-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97999-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97999-130">Schema Name</span></span>  <br/> |<span data-ttu-id="97999-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="97999-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97999-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97999-132">Validation File</span></span>  <br/> |<span data-ttu-id="97999-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="97999-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97999-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97999-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="97999-135">False</span><span class="sxs-lookup"><span data-stu-id="97999-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97999-136">См. также</span><span class="sxs-lookup"><span data-stu-id="97999-136">See also</span></span>



- [<span data-ttu-id="97999-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="97999-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

