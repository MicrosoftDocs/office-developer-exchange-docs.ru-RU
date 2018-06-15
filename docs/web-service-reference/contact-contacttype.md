---
title: Контакт (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: Элемент контакта указывает контакт в единого хранилища контактов.
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761726"
---
# <a name="contact-contacttype"></a><span data-ttu-id="6f264-103">Контакт (ContactType)</span><span class="sxs-lookup"><span data-stu-id="6f264-103">Contact (ContactType)</span></span>

<span data-ttu-id="6f264-104">Элемент **контактов** указывает контакт в единого хранилища контактов.</span><span class="sxs-lookup"><span data-stu-id="6f264-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 <span data-ttu-id="6f264-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="6f264-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f264-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6f264-106">Attributes and elements</span></span>

<span data-ttu-id="6f264-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6f264-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f264-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6f264-108">Attributes</span></span>

<span data-ttu-id="6f264-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6f264-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f264-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6f264-110">Child elements</span></span>

|<span data-ttu-id="6f264-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f264-111">**Element**</span></span>|<span data-ttu-id="6f264-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f264-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f264-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="6f264-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="6f264-114">Указывает имя отдельного.</span><span class="sxs-lookup"><span data-stu-id="6f264-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="6f264-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="6f264-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="6f264-116">Указывает имя компании.</span><span class="sxs-lookup"><span data-stu-id="6f264-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="6f264-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="6f264-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="6f264-118">Представляет коллекцию телефонных номеров контакта.</span><span class="sxs-lookup"><span data-stu-id="6f264-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="6f264-119">URL-адреса</span><span class="sxs-lookup"><span data-stu-id="6f264-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="6f264-120">Указывает массив URL-адресов для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f264-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="6f264-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="6f264-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="6f264-122">Указывает массив адресов извлеченные электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6f264-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="6f264-123">Адреса (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="6f264-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="6f264-124">Указывает массив элементов **адрес** .</span><span class="sxs-lookup"><span data-stu-id="6f264-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="6f264-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="6f264-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="6f264-126">Задает отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="6f264-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f264-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6f264-127">Parent elements</span></span>

|<span data-ttu-id="6f264-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f264-128">**Element**</span></span>|<span data-ttu-id="6f264-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f264-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f264-130">Контакты (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="6f264-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="6f264-131">Указывает массив контакты.</span><span class="sxs-lookup"><span data-stu-id="6f264-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f264-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="6f264-132">Remarks</span></span>

<span data-ttu-id="6f264-133">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6f264-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6f264-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f264-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f264-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6f264-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f264-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6f264-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f264-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6f264-137">Schema Name</span></span>  <br/> |<span data-ttu-id="6f264-138">Схема типа</span><span class="sxs-lookup"><span data-stu-id="6f264-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="6f264-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6f264-139">Validation File</span></span>  <br/> |<span data-ttu-id="6f264-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f264-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f264-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6f264-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6f264-142">См. также</span><span class="sxs-lookup"><span data-stu-id="6f264-142">See also</span></span>



- [<span data-ttu-id="6f264-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6f264-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
