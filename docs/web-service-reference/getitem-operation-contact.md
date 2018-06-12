---
title: Операции GetItem (контактов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: Операции GetItem используется для получения элементов контактов из хранилища Exchange.
ms.openlocfilehash: 8d7436421f0c54a49345e8ef6b37cb442bca4277
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762832"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="5fdb7-103">Операции GetItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-103">GetItem operation (contact)</span></span>

<span data-ttu-id="5fdb7-104">Операции GetItem используется для получения элементов контактов из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="5fdb7-105">Пример запроса GetItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5fdb7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5fdb7-106">Description</span></span>

<span data-ttu-id="5fdb7-107">Следующий пример демонстрирует получение элемента из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="5fdb7-108">Программа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5fdb7-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5fdb7-109">Comments</span></span>

<span data-ttu-id="5fdb7-110">Запрос на получение элемента из хранилища Exchange принимает одну форму для всех типов элементов.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-110">The request to get an item from the Exchange store takes the same form for all item types.</span></span> <span data-ttu-id="5fdb7-111">Так как различные элементы возвращать данные фигуры ответа на основе ответов на запросы для различных элементов будут отличаться.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-111">The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5fdb7-112">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="5fdb7-113">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="5fdb7-113">Request elements</span></span>

<span data-ttu-id="5fdb7-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5fdb7-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5fdb7-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="5fdb7-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="5fdb7-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5fdb7-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="5fdb7-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="5fdb7-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="5fdb7-118">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="5fdb7-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="5fdb7-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5fdb7-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="5fdb7-120">Успешные GetItem (контакт) ответа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="5fdb7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5fdb7-121">Description</span></span>

<span data-ttu-id="5fdb7-122">В следующем примере кода показано успешного ответа GetItem для **AllProperties**[BaseShape](baseshape.md).</span><span class="sxs-lookup"><span data-stu-id="5fdb7-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="5fdb7-123">Программа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5fdb7-124">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5fdb7-124">Comments</span></span>

<span data-ttu-id="5fdb7-125">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="5fdb7-126">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-126">Successful response elements</span></span>

<span data-ttu-id="5fdb7-127">В ответ на запрос GetItem с фигурой ответа **AllProperties** для элемента контактов используются следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="5fdb7-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5fdb7-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5fdb7-129">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="5fdb7-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="5fdb7-130">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5fdb7-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5fdb7-131">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5fdb7-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="5fdb7-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5fdb7-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5fdb7-133">Элементы</span><span class="sxs-lookup"><span data-stu-id="5fdb7-133">Items</span></span>](items.md)
    
- [<span data-ttu-id="5fdb7-134">Контакт</span><span class="sxs-lookup"><span data-stu-id="5fdb7-134">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="5fdb7-135">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5fdb7-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5fdb7-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5fdb7-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="5fdb7-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5fdb7-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="5fdb7-138">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="5fdb7-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="5fdb7-139">Body</span><span class="sxs-lookup"><span data-stu-id="5fdb7-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="5fdb7-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5fdb7-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="5fdb7-141">Размер</span><span class="sxs-lookup"><span data-stu-id="5fdb7-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="5fdb7-142">Важность</span><span class="sxs-lookup"><span data-stu-id="5fdb7-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="5fdb7-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="5fdb7-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="5fdb7-144">IsDraft</span><span class="sxs-lookup"><span data-stu-id="5fdb7-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="5fdb7-145">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="5fdb7-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="5fdb7-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="5fdb7-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="5fdb7-147">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="5fdb7-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="5fdb7-148">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="5fdb7-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="5fdb7-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5fdb7-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="5fdb7-150">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="5fdb7-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="5fdb7-151">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="5fdb7-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="5fdb7-152">FileAs</span><span class="sxs-lookup"><span data-stu-id="5fdb7-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="5fdb7-153">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="5fdb7-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="5fdb7-154">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5fdb7-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="5fdb7-155">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="5fdb7-156">Инициалы</span><span class="sxs-lookup"><span data-stu-id="5fdb7-156">Initials</span></span>](initials.md)
    
- [<span data-ttu-id="5fdb7-157">CompleteName</span><span class="sxs-lookup"><span data-stu-id="5fdb7-157">CompleteName</span></span>](completename.md)
    
- [<span data-ttu-id="5fdb7-158">FirstName</span><span class="sxs-lookup"><span data-stu-id="5fdb7-158">FirstName</span></span>](firstname.md)
    
- [<span data-ttu-id="5fdb7-159">Фамилия</span><span class="sxs-lookup"><span data-stu-id="5fdb7-159">LastName</span></span>](lastname.md)
    
- [<span data-ttu-id="5fdb7-160">Полное имя</span><span class="sxs-lookup"><span data-stu-id="5fdb7-160">FullName</span></span>](fullname.md)
    
- [<span data-ttu-id="5fdb7-161">Название организации</span><span class="sxs-lookup"><span data-stu-id="5fdb7-161">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="5fdb7-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5fdb7-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="5fdb7-163">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="5fdb7-164">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="5fdb7-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="5fdb7-165">Запись (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="5fdb7-166">Улица</span><span class="sxs-lookup"><span data-stu-id="5fdb7-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="5fdb7-167">Город</span><span class="sxs-lookup"><span data-stu-id="5fdb7-167">City</span></span>](city.md)
    
- [<span data-ttu-id="5fdb7-168">Состояние</span><span class="sxs-lookup"><span data-stu-id="5fdb7-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5fdb7-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="5fdb7-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="5fdb7-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="5fdb7-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="5fdb7-171">Запись (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="5fdb7-172">Название должности</span><span class="sxs-lookup"><span data-stu-id="5fdb7-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="5fdb7-173">Фамилия</span><span class="sxs-lookup"><span data-stu-id="5fdb7-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="5fdb7-174">Пример запроса недопустимый GetItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5fdb7-175">Описание</span><span class="sxs-lookup"><span data-stu-id="5fdb7-175">Description</span></span>

<span data-ttu-id="5fdb7-176">В следующем примере кода показано недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5fdb7-177">Программа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5fdb7-178">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5fdb7-178">Comments</span></span>

<span data-ttu-id="5fdb7-179">Идентификаторы элементов URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5fdb7-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="5fdb7-180">Отклик GetItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="5fdb7-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="5fdb7-181">Описание</span><span class="sxs-lookup"><span data-stu-id="5fdb7-181">Description</span></span>

<span data-ttu-id="5fdb7-182">В следующем примере кода показано возврату ошибки на запрос GetItem (контактов).</span><span class="sxs-lookup"><span data-stu-id="5fdb7-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5fdb7-183">Программа</span><span class="sxs-lookup"><span data-stu-id="5fdb7-183">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="5fdb7-184">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="5fdb7-184">Error response elements</span></span>

<span data-ttu-id="5fdb7-185">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5fdb7-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5fdb7-186">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5fdb7-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5fdb7-187">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="5fdb7-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="5fdb7-188">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5fdb7-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5fdb7-189">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5fdb7-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="5fdb7-190">MessageText</span><span class="sxs-lookup"><span data-stu-id="5fdb7-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5fdb7-191">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5fdb7-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5fdb7-192">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5fdb7-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5fdb7-193">Элементы</span><span class="sxs-lookup"><span data-stu-id="5fdb7-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="5fdb7-194">См. также</span><span class="sxs-lookup"><span data-stu-id="5fdb7-194">See also</span></span>



[<span data-ttu-id="5fdb7-195">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="5fdb7-195">GetItem operation</span></span>](getitem-operation.md)


- [<span data-ttu-id="5fdb7-196">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5fdb7-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

