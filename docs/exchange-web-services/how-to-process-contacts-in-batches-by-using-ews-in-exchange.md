---
title: Процесс контакты партиями с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 455f475b-cb19-4e7a-8ff3-92f7028fceb0
description: Узнайте, как создание, получение, обновление и удаление пакетов контактов в одном вызове с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 7dfbda7fe5e077f92bcf7ebd40af40d76c2d2d22
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761104"
---
# <a name="process-contacts-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="e200c-103">Процесс контакты партиями с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-103">Process contacts in batches by using EWS in Exchange</span></span>

<span data-ttu-id="e200c-104">Узнайте, как создание, получение, обновление и удаление пакетов контактов в одном вызове с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-104">Learn how to create, get, update, and delete batches of contacts in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="e200c-105">Можно использовать управляемый API EWS или делает веб-служб Exchange для работы с пакетами для контактов, чтобы сократить количество вызовов клиента к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-105">You can use the EWS Managed API or EWS to work with batches of contacts to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="e200c-106">При использовании управляемого интерфейса API веб-служб Exchange на создание, получение, обновление и удаление контактов в пакетах, используйте методы объекта [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , то время как при работе с одним контакты можно использовать методы объекта [контакта](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e200c-106">When you use the EWS Managed API to create, get, update, and delete contacts in batches, you use [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single contacts, you use [Contact](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="e200c-107">При использовании веб-служб Exchange для работы с одним контактом и пакетов контактов использовать такие же операции.</span><span class="sxs-lookup"><span data-stu-id="e200c-107">If you are using EWS, you use the same operations to work with both a single contact and batches of contacts.</span></span> 
  
<span data-ttu-id="e200c-108">**В таблице 1. Управляемый API EWS методы и операций веб-служб Exchange для работы с пакетами контактов**</span><span class="sxs-lookup"><span data-stu-id="e200c-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of contacts**</span></span>

|<span data-ttu-id="e200c-109">**Чтобы...**</span><span class="sxs-lookup"><span data-stu-id="e200c-109">**In order to…**</span></span>|<span data-ttu-id="e200c-110">**Используйте этот метод управляемый API EWS**</span><span class="sxs-lookup"><span data-stu-id="e200c-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="e200c-111">**Используйте эту операцию EWS**</span><span class="sxs-lookup"><span data-stu-id="e200c-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e200c-112">Создание контактов в пакетах</span><span class="sxs-lookup"><span data-stu-id="e200c-112">Create contacts in batches</span></span>  <br/> |[<span data-ttu-id="e200c-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="e200c-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e200c-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="e200c-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e200c-115">Получение контакты в пакетах</span><span class="sxs-lookup"><span data-stu-id="e200c-115">Get contacts in batches</span></span>  <br/> |<span data-ttu-id="e200c-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) или [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/ru-ru/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="e200c-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) or [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/ru-ru/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="e200c-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="e200c-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e200c-118">Обновлять контакты в пакетах</span><span class="sxs-lookup"><span data-stu-id="e200c-118">Update contacts in batches</span></span>  <br/> |[<span data-ttu-id="e200c-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="e200c-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/ru-ru/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e200c-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="e200c-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e200c-121">Удаление контактов в пакетах</span><span class="sxs-lookup"><span data-stu-id="e200c-121">Delete contacts in batches</span></span>  <br/> |[<span data-ttu-id="e200c-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="e200c-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/ru-ru/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e200c-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="e200c-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="e200c-124">В этой статье вы узнаете, как для выполнения основных задач для пакетов контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-124">In this article, you'll learn how to complete basic tasks for batches of contacts by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="e200c-125">Создание контактов партиями с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-125">Create contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="e200c-126"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-126"></span></span>

<span data-ttu-id="e200c-127">Контакты в пакетах можно создать с помощью метода управляемый API EWS [CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e200c-127">You can create contacts in batches by using the EWS Managed API [CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="e200c-128">В этом примере создается три [Contact](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) objects локально, добавляет рядом с каждым контактом в коллекцию, а затем вызывается метод **CreateItems** коллекция контактов.</span><span class="sxs-lookup"><span data-stu-id="e200c-128">This example creates three [Contact](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) objects locally, adds each contact to a collection, then calls the **CreateItems** method on the collection of contacts.</span></span> 
  
```cs
public static Collection<ItemId> CreateContactsInBatch(ExchangeService service)
{
    // These are unsaved local instances of a Contact object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Contact contact1 = new Contact(service);
    Contact contact2 = new Contact(service);
    Contact contact3 = new Contact(service);
    // Set the properties on the first contact.
    contact1.DisplayName = "Sadie Daniels";
    contact1.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("sadie@contoso.com");
    
    // Set the properties on the second contact.
    contact2.DisplayName = "Alfred Welker";
    contact2.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("alfred@contoso.com");
    // Set the properties on the third contact.
    contact3.DisplayName = "Hope Gross";
    contact3.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("hope@contoso.com");
    // Add the Contact objects to a collection.
    Collection<Contact> contactItems = new Collection<Contact>() { contact1, contact2, contact3 };
    // Create the batch of contacts on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(contactItems, WellKnownFolderName.Contacts, null, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created contacts.
    foreach (Contact contact in contactItems)
    {
        try
        {
            itemIds.Add(contact.Id);
            Console.WriteLine("Contact '{0}' created successfully.", contact.DisplayName);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating contact {0}: {1}", contact.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Determine whether the CreateItems method call completed successfully.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created contacts were successfully created in the Contacts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each contact.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (contact {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

## <a name="create-contacts-in-batches-by-using-ews"></a><span data-ttu-id="e200c-129">Создание контактов партиями с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-129">Create contacts in batches by using EWS</span></span>
<span data-ttu-id="e200c-130"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-130"></span></span>

<span data-ttu-id="e200c-131">Контакты в пакетах можно создать с помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="e200c-131">You can create contacts in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="e200c-132">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [создания контактов в пакетах](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="e200c-132">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create contacts in batches](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:CreateItem>
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:Items>
          <t:Contact>
            <t:DisplayName>Sadie Daniels</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">sadie@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Alfred Welker</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">alfred@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Hope Gross</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">hope@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
        </m:Items>
      </m:CreateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="e200c-133">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** для каждого нового контакта, который указывает, что рядом с каждым контактом был создан и сохранен успешно.</span><span class="sxs-lookup"><span data-stu-id="e200c-133">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new contacts, which indicates that each contact was created and saved successfully.</span></span> 
  
## <a name="get-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="e200c-134">Получить контакты в пакетах с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-134">Get contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="e200c-135"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-135"></span></span>

<span data-ttu-id="e200c-136">Контакты в пакетах можно получить с помощью метода управляемый API EWS [BindToItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e200c-136">You can get contacts in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="e200c-137">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-137">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchGetContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Create a property set that limits the properties returned by the Bind method to only those that are required.
            PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ContactSchema.DisplayName);
            // Get the items from the server.
            // This method call results in a GetItem call to EWS.
            ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
            // Instantiate a collection of Contact objects to populate from the values that are returned by the Exchange server.
            Collection<Contact> contactItems = new Collection<Contact>();
            foreach (GetItemResponse getItemResponse in response)
            {
                try
                {
                    Item item = getItemResponse.Item;
                    Contact contact = (Contact)item;
                    contactItems.Add(contact);
                    // Print out confirmation and the last eight characters of the item ID.
                    Console.WriteLine("Found item {0}.", contact.Id.ToString().Substring(144));
                }
                catch (Exception ex)
                {
                    Console.WriteLine("Exception while getting a contact: {0}", ex.Message);
                }
            }
            // Check for success of the BindToItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts retrieved successfully.");
                Console.WriteLine("\r\n");
            }
            return contactItems;
        }

```

## <a name="get-contacts-in-batches-by-using-ews"></a><span data-ttu-id="e200c-138">Получить контакты в пакетах с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-138">Get contacts in batches by using EWS</span></span>
<span data-ttu-id="e200c-139"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-139"></span></span>

<span data-ttu-id="e200c-140">Контакты можно получить в пакетах с помощью операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) веб-служб Exchange и код в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e200c-140">You can get contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="e200c-141">Это также запроса XML, управляемый API EWS отправляет при использовании управляемый API EWS для [получения контактов в пакетах](#bk_EWSMAGet).</span><span class="sxs-lookup"><span data-stu-id="e200c-141">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get contacts in batches](#bk_EWSMAGet).</span></span> <span data-ttu-id="e200c-142">Атрибут **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e200c-142">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetItem>
        <m:ItemShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="contacts:DisplayName" />
          </t:AdditionalProperties>
        </m:ItemShape>
        <m:ItemIds>
          <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
          <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
          <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
        </m:ItemIds>
      </m:GetItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="e200c-143">Сервер отвечает на запрос **GetItem** [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) сообщение, содержащее идентификатор и отображаемое имя для каждого из них запрошенные контактов.</span><span class="sxs-lookup"><span data-stu-id="e200c-143">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the ID and the display name for each of the requested contacts.</span></span> 
  
## <a name="update-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="e200c-144">Обновление контактов партиями с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-144">Update contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="e200c-145"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-145"></span></span>

<span data-ttu-id="e200c-146">Контакты в пакетах можно обновить с помощью метода управляемый API EWS [UpdateItems](http://msdn.microsoft.com/ru-ru/library/dd634705%28v=exchg.80%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e200c-146">You can update contacts in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/ru-ru/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="e200c-147">В предыдущем примере создается контакт, но не определяет пользователей, которые они работают.</span><span class="sxs-lookup"><span data-stu-id="e200c-147">The previous example creates the contact but does not specify who they work for.</span></span> <span data-ttu-id="e200c-148">В этом примере можно использовать код для обновления всех контактов, за один раз, чтобы включить их имя компании.</span><span class="sxs-lookup"><span data-stu-id="e200c-148">You can use the code in this example to update all your contacts at once to include their company name.</span></span> 
  
<span data-ttu-id="e200c-149">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchUpdateContactItems(ExchangeService service, Collection<Contact> contactItems)
        {
            // Update the company name of each contact locally.
            foreach (Contact contact in contactItems)
            {
                // Update the company name of the contact.
                contact.CompanyName = "Contoso";
                // Print out confirmation with the last eight characters of the item ID and the contact company name.
                Console.WriteLine("Updated local contact {0} with the company name '{1}'.", contact.Id.ToString().Substring(144), contact.CompanyName);
            }
            
            // Send the item updates to the server.
            // This method call results in an UpdateItem call to EWS.
            ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(contactItems, WellKnownFolderName.Contacts, ConflictResolutionMode.AutoResolve, null, null);
            // Verify the success of the UpdateItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts updated successfully.\r\n");
            }
            // If the method did not return success, print the result message for each contact.
            else
            {
                Console.WriteLine("All contacts were not successfully saved on the server.\r\n");
                int counter = 1;
                foreach (ServiceResponse resp in response)
                {
                    Console.WriteLine("Result for (contact {0}): {1}", counter, resp.Result);
                    Console.WriteLine("Error Code: {0}", resp.ErrorCode);
                    Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
                    counter++;
                }
            }
            return contactItems;
        }    

```

## <a name="update-contacts-in-batches-by-using-ews"></a><span data-ttu-id="e200c-150">Обновление контактов партиями с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-150">Update contacts in batches by using EWS</span></span>
<span data-ttu-id="e200c-151"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-151"></span></span>

<span data-ttu-id="e200c-152">Контакты в пакетах можно обновить с помощью операции [Getitem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="e200c-152">You can update contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="e200c-153">Это также запроса XML, управляемый API EWS отправляет при использовании управляемый API EWS для [контактов в пакетах обновления](#bk_EWSMAUpdate).</span><span class="sxs-lookup"><span data-stu-id="e200c-153">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update contacts in batches](#bk_EWSMAUpdate).</span></span> <span data-ttu-id="e200c-154">Атрибут **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e200c-154">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:UpdateItem ConflictResolution="AutoResolve">
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:ItemChanges>
          <t:ItemChange>
            <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
        </m:ItemChanges>
      </m:UpdateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="e200c-155">Сервер отвечает на запрос **UpdateItem** с [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) сообщения, которое содержит значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что каждый из обновления успешно сохранен на сервере.</span><span class="sxs-lookup"><span data-stu-id="e200c-155">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="e200c-156">В элементе [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) выводятся все конфликты.</span><span class="sxs-lookup"><span data-stu-id="e200c-156">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="e200c-157">Удаление контактов в пакетах с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-157">Delete contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="e200c-158"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-158"></span></span>

<span data-ttu-id="e200c-159">Контакты в пакетах можно удалить с помощью метода управляемый API EWS [DeleteItems](http://msdn.microsoft.com/ru-ru/library/dd635460%28v=exchg.80%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e200c-159">You can delete contacts in batches by using the [DeleteItems](http://msdn.microsoft.com/ru-ru/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="e200c-160">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e200c-160">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void BatchDeleteContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Delete the batch of contact objects.
            // This method call results in an DeleteItem call to EWS.
            ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
            // Check for success of the DeleteItems method call.
            // DeleteItems returns success even if it does not find all the item IDs.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("Contacts deleted successfully.\r\n");
            }
            // If the method did not return success, print a message.
            else
            {
                Console.WriteLine("Not all contacts deleted successfully.\r\n");
            }
        }

```

## <a name="delete-contacts-in-batches-by-using-ews"></a><span data-ttu-id="e200c-161">Удаление контактов партиями с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-161">Delete contacts in batches by using EWS</span></span>
<span data-ttu-id="e200c-162"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-162"></span></span>

<span data-ttu-id="e200c-163">Контакты в пакетах можно удалить с помощью операции [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="e200c-163">You can delete contacts in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="e200c-164">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [удаления контактов в пакетах](#bk_EWSMADelete).</span><span class="sxs-lookup"><span data-stu-id="e200c-164">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete contacts in batches](#bk_EWSMADelete).</span></span> <span data-ttu-id="e200c-165">Атрибут **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e200c-165">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:DeleteItem DeleteType="SoftDelete" AffectedTaskOccurrences="AllOccurrences">
        <m:ItemIds>
          <t:ItemId Id="ceJwYAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yY" />
          <t:ItemId Id="ceJwZAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yZ" />
          <t:ItemId Id="ceJwaAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51ya" />
        </m:ItemIds>
      </m:DeleteItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="e200c-166">Сервер отвечает на запрос **DeleteItem** [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** для каждого элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="e200c-166">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="e200c-167">Обратите внимание, что операция также возвращает успех, если не удалось найти идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="e200c-167">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="e200c-168">Проверка успешного завершения процесса пакетной обработки</span><span class="sxs-lookup"><span data-stu-id="e200c-168">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="e200c-169"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="e200c-169"></span></span>

<span data-ttu-id="e200c-170">Когда один или несколько контактов в пакетной запрос не удается обработать по запросу, возвращается сообщение об ошибке для каждого контакта, который не удалось и rest контакты в пакете обрабатываются как ожидалось.</span><span class="sxs-lookup"><span data-stu-id="e200c-170">When one or more contacts in a batched request can't be processed as requested, an error is returned for each contact that failed, and the rest of the contacts in the batch are processed as expected.</span></span> <span data-ttu-id="e200c-171">В пакетной обработке могут возникнуть ошибки при элемент был удален и поэтому не удается извлечь или обновить, а также если элемент перемещен в другую папку и таким образом имеет новый идентификатор элемента и не могут быть изменены с Идентификатором элемента отправлено.</span><span class="sxs-lookup"><span data-stu-id="e200c-171">Failures in batch processing can occur if the item was deleted, and therefore can't be retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="e200c-172">Сведения, приведенные в этом разделе показано, как получить дополнительные сведения об ошибке о сбоях в пакетной обработке контакты.</span><span class="sxs-lookup"><span data-stu-id="e200c-172">The information in this section shows how to get error details about failures in batch processing of contacts.</span></span>
  
<span data-ttu-id="e200c-173">Чтобы проверить успешность пакетной обработки с помощью управляемого интерфейса API веб-служб Exchange, можно проверить, что свойство [OverallResult](http://msdn.microsoft.com/ru-ru/library/dd634515%28v=exchg.80%29.aspx) [ServiceResponseCollection](http://msdn.microsoft.com/ru-ru/library/dd633715%28v=exchg.80%29.aspx) равен [ServiceResult.Success](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e200c-173">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/ru-ru/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/ru-ru/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="e200c-174">Если это так, все контакты обработаны успешно.</span><span class="sxs-lookup"><span data-stu-id="e200c-174">If so, all the contacts were processed successfully.</span></span> <span data-ttu-id="e200c-175">Если **OverallResult** не равно **ServiceResult.Success**, один или несколько контактов, не были успешно обработаны.</span><span class="sxs-lookup"><span data-stu-id="e200c-175">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the contacts were not processed successfully.</span></span> <span data-ttu-id="e200c-176">Каждый из объектов, возвращаемых **ServiceResponseCollection** содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="e200c-176">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="e200c-177">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="e200c-177">ErrorCode</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e200c-178">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e200c-178">ErrorDetails</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e200c-179">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="e200c-179">ErrorMessage</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e200c-180">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="e200c-180">ErrorProperties</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e200c-181">Результат</span><span class="sxs-lookup"><span data-stu-id="e200c-181">Result</span></span>](http://msdn.microsoft.com/ru-ru/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="e200c-182">Эти свойства содержат сведения о почему контакты не удалось обработать по запросу.</span><span class="sxs-lookup"><span data-stu-id="e200c-182">These properties contain information about why the contacts could not be processed as requested.</span></span> <span data-ttu-id="e200c-183">Примеры в этой статье распечатать **результатов**, **код ошибки**и **сообщение об ошибке** для каждого из них не удалось контакт.</span><span class="sxs-lookup"><span data-stu-id="e200c-183">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed contact.</span></span> <span data-ttu-id="e200c-184">Эти результаты можно использовать для изучения проблемы.</span><span class="sxs-lookup"><span data-stu-id="e200c-184">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="e200c-185">Для веб-служб Exchange Чтобы убедиться в успешности процесса пакетной, проверьте атрибут [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) для каждого элемента, обрабатываемых.</span><span class="sxs-lookup"><span data-stu-id="e200c-185">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="e200c-186">Ниже приведен базовая структура **ResponseMessageType**, базового типа, из которых все ответа полученных сообщений.</span><span class="sxs-lookup"><span data-stu-id="e200c-186">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="e200c-187">Если контакт не был успешно обработан атрибут **ResponseClass** , значение **успеха** , если контакт был успешно обработан или **Ошибка** .</span><span class="sxs-lookup"><span data-stu-id="e200c-187">The **ResponseClass** attribute is set to **Success** if the contact was processed successfully, or **Error** if the contact was not processed successfully.</span></span> <span data-ttu-id="e200c-188">Для контактов не возникает **Предупреждение** во время пакетной обработки.</span><span class="sxs-lookup"><span data-stu-id="e200c-188">For contacts, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="e200c-189">Если **ResponseClass** **Успех**, элемент [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , исходя из также всегда имеет значение **NoError**.</span><span class="sxs-lookup"><span data-stu-id="e200c-189">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="e200c-190">Если **ResponseClass** **ошибки**, необходимо проверить значения [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**и [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) элементы, чтобы определить причину ошибки.</span><span class="sxs-lookup"><span data-stu-id="e200c-190">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="e200c-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) не в настоящее время используется.</span><span class="sxs-lookup"><span data-stu-id="e200c-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e200c-192">См. также</span><span class="sxs-lookup"><span data-stu-id="e200c-192">See also</span></span>


- [<span data-ttu-id="e200c-193">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-193">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="e200c-194">Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e200c-194">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="e200c-195">В Exchange обработки элементов календаря в пакетах</span><span class="sxs-lookup"><span data-stu-id="e200c-195">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    

