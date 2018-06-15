---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: Элемент MailboxSearchScope указывает почтовый ящик и область поиска для поиска обнаружения.
ms.openlocfilehash: 657e6dfd4eb6c6c0eabb18546e7090c524e28e5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834297"
---
# <a name="mailboxsearchscope"></a><span data-ttu-id="7a89d-103">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="7a89d-103">MailboxSearchScope</span></span>

<span data-ttu-id="7a89d-104">Элемент **MailboxSearchScope** указывает почтовый ящик и область поиска для поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="7a89d-104">The **MailboxSearchScope** element specifies a mailbox and a search scope for a discovery search.</span></span> 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

<span data-ttu-id="7a89d-105">**MailboxSearchScopeType**</span><span class="sxs-lookup"><span data-stu-id="7a89d-105">**MailboxSearchScopeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7a89d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a89d-106">Attributes and elements</span></span>

<span data-ttu-id="7a89d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7a89d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a89d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a89d-108">Attributes</span></span>

<span data-ttu-id="7a89d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a89d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a89d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a89d-110">Child elements</span></span>

<span data-ttu-id="7a89d-111">[Почтовый ящик (string)](mailbox-string.md) | [область поиска](searchscope.md)</span><span class="sxs-lookup"><span data-stu-id="7a89d-111">[Mailbox (string)](mailbox-string.md) | [SearchScope](searchscope.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a89d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a89d-112">Parent elements</span></span>

[<span data-ttu-id="7a89d-113">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="7a89d-113">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
  
## <a name="remarks"></a><span data-ttu-id="7a89d-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="7a89d-114">Remarks</span></span>

<span data-ttu-id="7a89d-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7a89d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a89d-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a89d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a89d-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a89d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a89d-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a89d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a89d-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a89d-119">Schema name</span></span>  <br/> |<span data-ttu-id="7a89d-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7a89d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a89d-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a89d-121">Validation file</span></span>  <br/> |<span data-ttu-id="7a89d-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a89d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a89d-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a89d-123">Can be empty</span></span>  <br/> ||
   
