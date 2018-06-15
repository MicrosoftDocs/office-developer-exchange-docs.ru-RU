---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: Элемент InboxRules представляет собой массив из правил в почтовом ящике пользователя.
ms.openlocfilehash: 47fcad5dde06f3af9fbae7e70adbfd8b225081c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833899"
---
# <a name="inboxrules"></a><span data-ttu-id="66d0f-103">InboxRules</span><span class="sxs-lookup"><span data-stu-id="66d0f-103">InboxRules</span></span>

<span data-ttu-id="66d0f-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **InboxRules** представляет собой массив из правил в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="66d0f-104">The **InboxRules** element represents an array of rules in the user's mailbox.</span></span> 
  
[<span data-ttu-id="66d0f-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="66d0f-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="66d0f-106">InboxRules</span><span class="sxs-lookup"><span data-stu-id="66d0f-106">InboxRules</span></span>](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 <span data-ttu-id="66d0f-107">**ArrayOfRulesType**</span><span class="sxs-lookup"><span data-stu-id="66d0f-107">**ArrayOfRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66d0f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="66d0f-108">Attributes and elements</span></span>

<span data-ttu-id="66d0f-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="66d0f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66d0f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="66d0f-110">Attributes</span></span>

<span data-ttu-id="66d0f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="66d0f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66d0f-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="66d0f-112">Child elements</span></span>

|<span data-ttu-id="66d0f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="66d0f-113">**Element**</span></span>|<span data-ttu-id="66d0f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="66d0f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66d0f-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="66d0f-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="66d0f-116">Содержит одно правило и представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="66d0f-116">Contains a single rule and represents a rule in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66d0f-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="66d0f-117">Parent elements</span></span>

|<span data-ttu-id="66d0f-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="66d0f-118">**Element**</span></span>|<span data-ttu-id="66d0f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="66d0f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66d0f-120">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="66d0f-120">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="66d0f-121">Определяет ответ на запрос [Операция GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="66d0f-121">Defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66d0f-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="66d0f-122">Text value</span></span>

<span data-ttu-id="66d0f-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="66d0f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66d0f-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="66d0f-124">Remarks</span></span>

<span data-ttu-id="66d0f-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="66d0f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66d0f-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="66d0f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66d0f-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="66d0f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66d0f-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="66d0f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="66d0f-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="66d0f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66d0f-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="66d0f-130">Validation File</span></span>  <br/> |<span data-ttu-id="66d0f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66d0f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66d0f-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="66d0f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="66d0f-133">True</span><span class="sxs-lookup"><span data-stu-id="66d0f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66d0f-134">См. также</span><span class="sxs-lookup"><span data-stu-id="66d0f-134">See also</span></span>



[<span data-ttu-id="66d0f-135">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="66d0f-135">GetInboxRules</span></span>](getinboxrules.md)
  
[<span data-ttu-id="66d0f-136">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="66d0f-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)


- [<span data-ttu-id="66d0f-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="66d0f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
