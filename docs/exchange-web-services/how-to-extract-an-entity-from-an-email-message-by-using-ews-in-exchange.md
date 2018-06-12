---
title: Извлечь сущности из сообщения электронной почты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6396b009-5f6e-41eb-a75a-224d43e864ae
description: Узнайте, как получить данные из текста сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: d3d5c4b756347a4cedede184709884d5ed8f08b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761007"
---
# <a name="extract-an-entity-from-an-email-message-by-using-ews-in-exchange"></a>Извлечь сущности из сообщения электронной почты с помощью веб-служб Exchange в Exchange

Узнайте, как получить данные из текста сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Управляемый API EWS или веб-служб Exchange можно использовать для доступа к адреса, контакты, адреса электронной почты, предложения о собрании, номера телефонов, задачи и URL-адресов, Exchange server извлекает из сообщений электронной почты. Затем можно использовать эти сведения для новых приложений или предложить дальнейшие действия в существующие приложения. К примеру контактного лица, предложения о собрании или предложения задачи, идентифицируемым в сообщение электронной почты, приложение может предложить, что создается новый элемент с предварительно заполненными данными. С помощью извлеченного сущностей, вы может капитализации цель за данные и помогают пользователям легко интегрировать их содержимое сообщения электронной почты в предусматривающей действие результатов.
  
Извлечение сущностей для адресов, контакты, адреса электронной почты, предложения о собрании, телефонных номеров, задачи и URL-адреса, уже созданных для всех элементов в хранилище Exchange. Если вы используете управляемый API веб-служб Exchange, свойство [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) извлекает сущности для вас в вызове метода [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) . Если вы используете веб-служб Exchange, элемент [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) получает все извлеченные сущности для вас в вызова операции [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) . После получения результатов сущности, извлеченные справляются каждого семейства сайтов сущности для сбора необходимых данных. Например если предложения о собрании было извлечено, можно извлечь тему предложенного собрания, список участников, время начала и время окончания. 
  
**В таблице 1. Управляемый API EWS свойства и элементы веб-служб Exchange, которые содержат извлеченные сущности**

|**Извлеченный объект**|**Свойство управляемый API EWS**|**Элемент веб-служб Exchange**|
|:-----|:-----|:-----|
|Адреса  <br/> |[EntityExtractionResult.Addresses](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[Адреса](http://msdn.microsoft.com/library/0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e%28Office.15%29.aspx) <br/> |
|Контакты  <br/> |[EntityExtractionResult.Contacts](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.contacts%28v=exchg.80%29.aspx) <br/> |[Контакты](http://msdn.microsoft.com/library/a2c1e833-5f8c-438d-bad7-bb5dcc29ca9e%28Office.15%29.aspx) <br/> |
|Адрес электронной почты  <br/> |[EntityExtractionResult.EmailAddresses](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.emailaddresses%28v=exchg.80%29.aspx) <br/> |[EmailAddresses](http://msdn.microsoft.com/library/2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3%28Office.15%29.aspx) <br/> |
|Предложения о собрании  <br/> |[EntityExtractionResult.MeetingSuggestions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.meetingsuggestions%28v=exchg.80%29.aspx) <br/> |[MeetingSuggestions](http://msdn.microsoft.com/library/c99e9a60-9e38-425d-ad03-47c8917f41da%28Office.15%29.aspx) <br/> |
|Номера телефонов  <br/> |[EntityExtractionResult.PhoneNumbers](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.phonenumbers%28v=exchg.80%29.aspx) <br/> |[PhoneNumbers](http://msdn.microsoft.com/library/9ff6ae98-34a1-47f7-bde5-608251a789f7%28Office.15%29.aspx) <br/> |
|Предложения задач  <br/> |[EntityExtractionResult.TaskSuggestions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[TaskSuggestions](http://msdn.microsoft.com/library/7d3c6314-2a5c-4fc3-b5f9-ae6d4946aac3%28Office.15%29.aspx) <br/> |
|URL-адреса  <br/> |[EntityExtractionResult.Urls](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[URL-адреса](http://msdn.microsoft.com/library/c39744ea-0cee-4954-8653-8279d6b10161%28Office.15%29.aspx) <br/> |
   
Так как извлечение сущностей полагается на естественном языке распознавания, распознавания сущности может быть недетерминированным и успеха в некоторых случаях основывается на контексте. Для демонстрации, как работает распознавания естественном языке, примеров, описанных в этой статье использование следующих электронной почты как входные данные.
  
 `From: Ronnie Sturgis`
  
 `To: Sadie Daniels`
  
 `Subject: Dinner party`
  
 `Hi Sadie`
  
 `Are you free this Friday at 7 to join us for a dinner party at our house?`
  
 `We're at 789 International Blvd, St Paul MN 55104.`
  
 `Our number is 612-555-0158 if you have trouble finding it.`
  
 `Please RSVP to either myself or Mara (mara@contoso.com) before Friday morning. Best for you organics (http://www.bestforyouorganics.com) will be catering so we can fully enjoy ourselves!`
  
 `Also, can you forward this to Magdalena? I don't have her contact information.`
  
 `See you then!`
  
 `Ronnie`
  
## <a name="extract-all-entities-from-an-email-by-using-the-ews-managed-api"></a>Извлеките все объекты из сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_extractewsma"> </a>

В следующем примере кода показано, как отобразить все сущности, извлеченные на сервере, с помощью метода [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) , затем перечисления в каждой из извлеченных объектов и их свойств. 
  
В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и этот **идентификатор элемента** — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) для сообщения электронной почты для перемещения или копирования. 
  
```cs
public static void ExtractEntities(ExchangeService service, ItemId ItemId)
{
    // Create a property set that limits the properties returned 
    // by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.EntityExtractionResult);
    // Get the item from the server.
    // This method call results in an GetItem call to EWS.
    Item item = Item.Bind(service, ItemId, propSet);
    Console.WriteLine("The following entities have been extracted from the message:");
    Console.WriteLine(" ");
    // If address entities are extracted from the message, print the results.
    if (item.EntityExtractionResult != null)
    {
        if (item.EntityExtractionResult.Addresses != null)
        {
            Console.WriteLine("--------------------Addresses---------------------------");
            foreach (AddressEntity address in item.EntityExtractionResult.Addresses)
            {
                Console.WriteLine("Address: {0}", address.Address);
            }
            Console.WriteLine(" ");
        }
        // If contact entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Contacts != null)
        {
            Console.WriteLine("--------------------Contacts----------------------------");
            foreach (ContactEntity contact in item.EntityExtractionResult.Contacts)
            {
                Console.WriteLine("Addresses:       {0}", contact.Addresses);
                Console.WriteLine("Business name:   {0}", contact.BusinessName);
                Console.WriteLine("Contact string:  {0}", contact.ContactString);
                Console.WriteLine("Email addresses: {0}", contact.EmailAddresses);
                Console.WriteLine("Person name:     {0}", contact.PersonName);
                Console.WriteLine("Phone numbers:   {0}", contact.PhoneNumbers);
                Console.WriteLine("URLs:            {0}", contact.Urls);
            }
            Console.WriteLine(" ");
        }
        // If email address entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.EmailAddresses != null)
        {
            Console.WriteLine("--------------------Email addresses---------------------");
            foreach (EmailAddressEntity email in item.EntityExtractionResult.EmailAddresses)
            {
                Console.WriteLine("Email addresses: {0}", email.EmailAddress);
            }
            Console.WriteLine(" ");
        }
        // If meeting suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.MeetingSuggestions != null)
        {
            Console.WriteLine("--------------------Meeting suggestions-----------------");
            foreach (MeetingSuggestion meetingSuggestion in item.EntityExtractionResult.MeetingSuggestions)
            {
                Console.WriteLine("Meeting subject:  {0}", meetingSuggestion.Subject);
                Console.WriteLine("Meeting string:   {0}", meetingSuggestion.MeetingString);
                foreach (EmailUserEntity attendee in meetingSuggestion.Attendees)
                {
                    Console.WriteLine("Attendee name:    {0}", attendee.Name);
                    Console.WriteLine("Attendee user ID: {0}", attendee.UserId);
                }
                Console.WriteLine("Start time:       {0}", meetingSuggestion.StartTime);
                Console.WriteLine("End time:         {0}", meetingSuggestion.EndTime);
                Console.WriteLine("Location:         {0}", meetingSuggestion.Location);
            }
            Console.WriteLine(" ");
        }
        // If phone number entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.PhoneNumbers != null)
        {
            Console.WriteLine("--------------------Phone numbers-----------------------");
            foreach (PhoneEntity phone in item.EntityExtractionResult.PhoneNumbers)
            {
                Console.WriteLine("Original phone string:  {0}", phone.OriginalPhoneString);
                Console.WriteLine("Phone string:           {0}", phone.PhoneString);
                Console.WriteLine("Type:                   {0}", phone.Type);
            }
            Console.WriteLine(" ");
        }
        // If task suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.TaskSuggestions != null)
        {
            Console.WriteLine("--------------------Task suggestions--------------------");
            foreach (TaskSuggestion task in item.EntityExtractionResult.TaskSuggestions)
            {
                foreach (EmailUserEntity assignee in task.Assignees)
                {
                    Console.WriteLine("Assignee name:    {0}", assignee.Name);
                    Console.WriteLine("Assignee user ID: {0}", assignee.UserId);
                }
                Console.WriteLine("Task string:      {0}", task.TaskString);
            }
            Console.WriteLine(" ");
        }
        // If URL entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Urls != null)
        {
            Console.WriteLine("--------------------URLs--------------------------------");
            foreach (UrlEntity url in item.EntityExtractionResult.Urls)
            {
                Console.WriteLine("URL: {0}", url.Url);
            }
            Console.WriteLine(" ");
        }
    }
    // If no entities are extracted from the message, print the result.
    else if (item.EntityExtractionResult == null)
    {
        Console.WriteLine("No entities extracted");
    }
}
```

Следующие результаты выводятся на консоль.
  
```text
The following entities have been extracted from the message:
 
--------------------Addresses---------------------------
Address: 789 International Blvd, St Paul MN 55104
 
--------------------Contacts----------------------------
Addresses:       
Business name:   
Contact string:  Mara (mara@contoso.com)
Email addresses: mara@contoso.com
Person name:     Mara
Phone numbers:   
URLs:            
 
--------------------Email addresses---------------------
Email addresses: mara@contoso.com
 
--------------------Meeting suggestions-----------------
Meeting subject:  dinner party
Meeting string:   Are you free this Friday at 7 to join us for a dinner party at our house?
Attendee name:    Ronnie Sturgis
Attendee user ID: ronnie@contoso.com
Attendee name:    Sadie Daniels
Attendee user ID: sadie@cntoso.com
Start time:       10/1/0104 2:00:00 PM
End time:         10/1/0104 2:30:00 PM
Location:         
 
--------------------Phone numbers-----------------------
Original phone string:  612-555-0158
Phone string:           6125550158
Type:                   Unspecified
 
--------------------Task suggestions--------------------
Assignee name:    Sadie Daniels
Assignee user ID: sadie@contoso.com
Task string:      Also, can you forward this to Magdalena?
 
--------------------URLs--------------------------------
URL: http://www.bestforyouorganics.com
```

Обратите внимание на то, что все адреса, контакты, адреса электронной почты, номера телефонов, задачи и URL-адреса были извлечены как ожидалось. Тем не менее, предложения о собрании немного сложнее. Обратите внимание, время начала и время окончания собрания, не ожиданиям. Время начала в сообщение электронной почты «в этом пятницу в 7», но извлеченного значения для времени начала 10/1/0104 2:00:00 PM. Это так, как время начала и время окончания, извлеченные сервером — закодированный даты. Дополнительные сведения об интерпретации значений **даты и времени** в предложений о собрании, можно [[MS-OXCEXT]: клиент расширения объекта протокола](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).
  
## <a name="extract-all-entities-from-an-email-by-using-ews"></a>Извлеките все объекты из сообщения электронной почты с помощью веб-служб Exchange
<a name="bk_extractews"> </a>

В следующем примере кода показано, как использовать операции [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) и элемент [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) для извлечения сущностей, извлеченные из элемента. 
  
Это также запроса XML, отправляемого управляемый API веб-служб Exchange, при использовании метода **привязки** , чтобы [извлечь все сущности из сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange](#bk_extractewsma).
  
Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) укорочено для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:EntityExtractionResult" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="sVC5AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **GetItem** [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно извлечен. Ответ также включает в себя **EntityExtractionResult** для каждого извлеченный объект. 
  
Значение элемента **ItemId** укорочено для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="sVC5AAA="
                        ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAOOqJN" />
              <t:EntityExtractionResult>
                <t:Addresses>
                  <t:AddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Address>789 International Blvd, St Paul MN 55104</t:Address>
                  </t:AddressEntity>
                </t:Addresses>
                <t:MeetingSuggestions>
                  <t:MeetingSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:Attendees>
                      <t:EmailUser>
                        <t:Name>Ronnie Sturgis</t:Name>
                        <t:UserId>ronnie@contoso.com</t:UserId>
                      </t:EmailUser>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Attendees>
                    <t:Subject>dinner party</t:Subject>
                    <t:MeetingString>Are you free this Friday at 7 to join us for a dinner party at our house?</t:MeetingString>
                    <t:StartTime>0104-10-01T19:00:00Z</t:StartTime>
                    <t:EndTime>0104-10-01T19:30:00Z</t:EndTime>
                  </t:MeetingSuggestion>
                </t:MeetingSuggestions>
                <t:TaskSuggestions>
                  <t:TaskSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:TaskString>Also, can you forward this to Magdalena?</t:TaskString>
                    <t:Assignees>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Assignees>
                  </t:TaskSuggestion>
                </t:TaskSuggestions>
                <t:EmailAddresses>
                  <t:EmailAddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                  </t:EmailAddressEntity>
                </t:EmailAddresses>
                <t:Contacts>
                  <t:Contact>
                    <t:Position>LatestReply</t:Position>
                    <t:PersonName>Mara</t:PersonName>
                    <t:EmailAddresses>
                      <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                    </t:EmailAddresses>
                    <t:ContactString>Mara (mara@contoso.com</t:ContactString>
                  </t:Contact>
                </t:Contacts>
                <t:Urls>
                  <t:UrlEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Url>http://www.bestforyouorganics.com</t:Url>
                  </t:UrlEntity>
                </t:Urls>
                <t:PhoneNumbers>
                  <t:Phone>
                    <t:Position>LatestReply</t:Position>
                    <t:OriginalPhoneString>612-555-0158</t:OriginalPhoneString>
                    <t:PhoneString>6125550158</t:PhoneString>
                    <t:Type>Unspecified</t:Type>
                  </t:Phone>
                </t:PhoneNumbers>
              </t:EntityExtractionResult>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

Обратите внимание на то, что все адреса, контакты, адреса электронной почты, номера телефонов, задачи и URL-адреса были извлечены как ожидалось. Тем не менее, предложения о собрании немного сложнее. Обратите внимание, время начала и время окончания собрания, не ожиданиям. Время начала в сообщение электронной почты было «этот пятницу в 7», но извлеченное значение времени начала — 10/1/0104 2:00:00 PM. Это так, как время начала и время окончания, извлеченные сервером — закодированный даты. Дополнительные сведения об интерпретации значений **даты и времени** в предложений о собрании, можно [[MS-OXCEXT]: клиент расширения объекта протокола](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).
  
## <a name="see-also"></a>См. также

- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
- [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx)    
- [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx)
    
