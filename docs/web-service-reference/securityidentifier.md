---
title: секуритидентифиер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: Элемент Секуритидентифиер представляет форму языка определения дескрипторов безопасности (SID).
ms.openlocfilehash: c55e4a7f7f0b8f8a40e6fcaf8d18e253a6da2679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468805"
---
# <a name="securityidentifier"></a><span data-ttu-id="36f1f-103">секуритидентифиер</span><span class="sxs-lookup"><span data-stu-id="36f1f-103">SecurityIdentifier</span></span>

<span data-ttu-id="36f1f-104">Элемент **секуритидентифиер** представляет форму языка определения дескрипторов безопасности ( [SID](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="36f1f-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="36f1f-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="36f1f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36f1f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36f1f-106">Attributes and elements</span></span>

<span data-ttu-id="36f1f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="36f1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36f1f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36f1f-108">Attributes</span></span>

<span data-ttu-id="36f1f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36f1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36f1f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36f1f-110">Child elements</span></span>

<span data-ttu-id="36f1f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36f1f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36f1f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36f1f-112">Parent elements</span></span>

|<span data-ttu-id="36f1f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36f1f-113">**Element**</span></span>|<span data-ttu-id="36f1f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36f1f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36f1f-115">граупидентифиер</span><span class="sxs-lookup"><span data-stu-id="36f1f-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="36f1f-116">Представляет один идентификатор безопасности и атрибут для группы объектов Active Directory, членом которой является учетная запись.</span><span class="sxs-lookup"><span data-stu-id="36f1f-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="36f1f-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="36f1f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="36f1f-118">рестриктедграупидентифиер</span><span class="sxs-lookup"><span data-stu-id="36f1f-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="36f1f-119">Представляет идентификатор и атрибуты безопасности группы для группы с ограниченным доступом в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="36f1f-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36f1f-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="36f1f-120">Remarks</span></span>

<span data-ttu-id="36f1f-121">Этот элемент используется в заголовке протокола SOAP.</span><span class="sxs-lookup"><span data-stu-id="36f1f-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="36f1f-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="36f1f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36f1f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36f1f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36f1f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36f1f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36f1f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36f1f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="36f1f-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="36f1f-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="36f1f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36f1f-127">Validation File</span></span>  <br/> |<span data-ttu-id="36f1f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36f1f-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36f1f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36f1f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="36f1f-130">False</span><span class="sxs-lookup"><span data-stu-id="36f1f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36f1f-131">См. также</span><span class="sxs-lookup"><span data-stu-id="36f1f-131">See also</span></span>



- [<span data-ttu-id="36f1f-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36f1f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

