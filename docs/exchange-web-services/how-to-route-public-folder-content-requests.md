---
title: Маршрутизация запросов к содержимому общедоступных папок
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Все запросы для общих папок, включающих содержимое общих папок необходимость направляться в почтовый ящик общедоступных папок, в которой содержится контент для целевой папке. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки X AnchorMailbox и X-PublicFolderMailbox для определенного значения.
ms.openlocfilehash: 64fafecb9882b17a3394e54640df78f7aa180343
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354024"
---
# <a name="route-public-folder-content-requests"></a><span data-ttu-id="a7e39-104">Маршрутизация запросов к содержимому общедоступных папок</span><span class="sxs-lookup"><span data-stu-id="a7e39-104">Route public folder content requests</span></span>

<span data-ttu-id="a7e39-105">Все запросы для общих папок, включающих содержимое общих папок необходимость направляться в почтовый ящик общедоступных папок, в которой содержится контент для целевой папке.</span><span class="sxs-lookup"><span data-stu-id="a7e39-105">All requests for public folder information that involve the content of the public folder need to be routed to the public folder mailbox that holds the content for the target folder.</span></span> <span data-ttu-id="a7e39-106">Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки **X AnchorMailbox** и **X-PublicFolderMailbox** для определенного значения.</span><span class="sxs-lookup"><span data-stu-id="a7e39-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values.</span></span> 
  
<span data-ttu-id="a7e39-107">Следующая таблица содержит обзор процесса:</span><span class="sxs-lookup"><span data-stu-id="a7e39-107">The following table provides an overview of the process:</span></span>
  
<span data-ttu-id="a7e39-108">**Обзор общих папок**</span><span class="sxs-lookup"><span data-stu-id="a7e39-108">**Public folder overview**</span></span>

|<span data-ttu-id="a7e39-109">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7e39-109">Header</span></span>|<span data-ttu-id="a7e39-110">Что нужно сделать?</span><span class="sxs-lookup"><span data-stu-id="a7e39-110">What do I need?</span></span>|<span data-ttu-id="a7e39-111">Как его получить?</span><span class="sxs-lookup"><span data-stu-id="a7e39-111">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a7e39-112">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="a7e39-112">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="a7e39-113">1. [X-AnchorMailbox и X PublicFolderInformation значения](how-to-route-public-folder-hierarchy-requests.md) для почтового ящика иерархии общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="a7e39-113">1. [The X-AnchorMailbox and X-PublicFolderInformation values ](how-to-route-public-folder-hierarchy-requests.md) for the public folder hierarchy mailbox.</span></span><br/><br/><span data-ttu-id="a7e39-114">2. идентификатор GUID почтового ящика общедоступных папок с содержимым почтового ящика, которое передается для службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a7e39-114">2. The GUID of the public folder mailbox that contains the mailbox content, which is sent to the Autodiscover service.</span></span><br/><br/>  <span data-ttu-id="a7e39-115">**AutoDiscoverSMTPAddress** в ответе Autodisover становится значение заголовка **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="a7e39-115">The **AutoDiscoverSMTPAddress** in the Autodisover response becomes the value of the **X-AnchorMailbox** header.</span></span>  <br/> <span data-ttu-id="a7e39-116">![ЗАДАЧА](media/Ex15_PF_PFContent.png)</span><span class="sxs-lookup"><span data-stu-id="a7e39-116">![TODO](media/Ex15_PF_PFContent.png)</span></span>| <span data-ttu-id="a7e39-117">1. Используйте в примере кода в этой статье, который [реализует управляемый API веб-служб Exchange](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="a7e39-117">1. Use the code example in this article, which [implements the EWS Managed API](#bk_determineguidewsma).</span></span> <span data-ttu-id="a7e39-118">Или [Используйте веб-служб Exchange](#bk_determineguidews) и преобразования результатов, чтобы получить идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="a7e39-118">Or [use EWS](#bk_determineguidews) and convert your results to obtain a GUID.</span></span><br/><br/><span data-ttu-id="a7e39-119">2. [выполнения запроса автоматического обнаружения](#bk_makeautodrequest) с помощью идентификатора GUID, а также имя домена.</span><span class="sxs-lookup"><span data-stu-id="a7e39-119">2. [Make an Autodiscover request](#bk_makeautodrequest) by using the GUID plus the domain name.</span></span><br/><br/><span data-ttu-id="a7e39-120">3. Используйте значение элемента **AutoDiscoverSMTPAddress** , возвращаемого в ответе автообнаружения для [заполнения значения заголовков](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="a7e39-120">3. Use the value of the **AutoDiscoverSMTPAddress** element returned in the Autodiscover response to [populate the value of the headers](#bk_setheadervalues).</span></span>  <br/> |
|<span data-ttu-id="a7e39-121">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="a7e39-121">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="a7e39-122">На работу, значение X-PublicFolderMailbox — то же, что значение X-AnchorMailbox!</span><span class="sxs-lookup"><span data-stu-id="a7e39-122">Your work is done, the X-PublicFolderMailbox value is the same as the X-AnchorMailbox value!</span></span>  <br/> |<span data-ttu-id="a7e39-123">У вас уже есть его!</span><span class="sxs-lookup"><span data-stu-id="a7e39-123">You already have it!</span></span>  <br/> |
   
<span data-ttu-id="a7e39-124">После определения значения заголовка включайте их [во время внесения запросов контента общей папки](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="a7e39-124">After you have determined the header values, include them [when you make public folder content requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="a7e39-125">Действия, описанные в этой статье относятся только к запросов контента общей папки.</span><span class="sxs-lookup"><span data-stu-id="a7e39-125">The steps in this article are specific to public folder content requests.</span></span> <span data-ttu-id="a7e39-126">Чтобы определить, является ли запрос иерархии общедоступных папок или содержимого запроса, обратитесь к разделу [маршрутизации запросов общих папок](public-folder-access-with-ews-in-exchange.md#bk_routing).</span><span class="sxs-lookup"><span data-stu-id="a7e39-126">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>

<span data-ttu-id="a7e39-127"><a name="bk_determineguidewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a7e39-127"></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a><span data-ttu-id="a7e39-128">Определите идентификатор GUID почтового ящика общедоступных папок с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="a7e39-128">Determine the GUID of the public folder mailbox by using the EWS Managed API</span></span>


<span data-ttu-id="a7e39-129">Для определения идентификатора GUID почтового ящика содержимого общей папки, используйте приведенный ниже код, который выполняет следующие:</span><span class="sxs-lookup"><span data-stu-id="a7e39-129">To determine the GUID of the public folder content mailbox, use the following code example, which does the following:</span></span> 
  
- <span data-ttu-id="a7e39-130">Используется в заголовках **X-AnchorMailbox** и **X PublicFolderInformation** загрузки [маршрутизации](how-to-route-public-folder-hierarchy-requests.md)запросов иерархии общих папок.</span><span class="sxs-lookup"><span data-stu-id="a7e39-130">Uses the **X-AnchorMailbox** and **X-PublicFolderInformation** headers you retrieved by [routing public folder hierarchy requests](how-to-route-public-folder-hierarchy-requests.md).</span></span>
    
- <span data-ttu-id="a7e39-131">Вызывает метод управляемый API EWS [FindFolders](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) и включает в себя запрос для свойства **PR_REPLICA_LIST** (0x66980102)</span><span class="sxs-lookup"><span data-stu-id="a7e39-131">Calls the EWS Managed API [FindFolders](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method, and includes a request for the **PR_REPLICA_LIST** (0x66980102) property</span></span> 
    
<span data-ttu-id="a7e39-132">Значение **PR_REPLICA_LIST** определяет идентификатор GUID почтового ящика общей папки, который содержит содержимое папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a7e39-132">The **PR_REPLICA_LIST** value identifies the mailbox GUID of the public folder mailbox that has the content for the folder.</span></span> <span data-ttu-id="a7e39-133">Свойство **PR_REPLICA_LIST** является массив байтов, но приводится как код GUID для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="a7e39-133">The **PR_REPLICA_LIST** property is a byte array, but is cast as a GUID for this scenario.</span></span> <span data-ttu-id="a7e39-134">Идентификатор GUID и имя домена объединяется адрес, на котором для вызова службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a7e39-134">The GUID and the domain name are concatenated to form the address on which to call Autodiscover.</span></span> 
  
<span data-ttu-id="a7e39-135">В этом примере предполагается, что `service` — это объект [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для пользователя почтового ящика, `PFHAnchorHeader` и `PFHMailboxHeader` значения заголовков **X AnchorMailbox** и **X-PublicFolderMailbox** и домен — это имя домена, используемого клиент.</span><span class="sxs-lookup"><span data-stu-id="a7e39-135">This example assumes that  `service` is the [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox user,  `PFHAnchorHeader` and  `PFHMailboxHeader` are the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers, and domain is the domain name used by the tenant.</span></span> 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

<span data-ttu-id="a7e39-136">Если ошибка «не удалось выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="a7e39-136">If you received the error "The request failed.</span></span> <span data-ttu-id="a7e39-137">Базовое соединение закрыто: не удается установить отношение доверия для безопасного канала SSL/TLS», необходимо [Добавить вызов метода обратного вызова проверки](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="a7e39-137">The underlying connection was closed: Could not establish trust relationship for the SSL/TLS secure channel", you'll need to [add a call to a validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> <span data-ttu-id="a7e39-138">В примере кода включается заполнитель и комментарий для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7e39-138">A placeholder and comment for that method is included in the code example.</span></span>
  
<span data-ttu-id="a7e39-139">Если GUID почтового ящика является общим для всех общих папок в корне общей папки, в примере указывается адрес для [вызова службы автообнаружения](#bk_makeautodrequest) в консоли вывода и как возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="a7e39-139">If the mailbox GUID is the same for all the public folders under the public folder root, the example indicates the address to use when [calling Autodiscover](#bk_makeautodrequest) in the console output and as the return value.</span></span> <span data-ttu-id="a7e39-140">Идентификатор GUID почтового ящика не является общим для всех общих папок в корне общей папки, требуется ли [выполнения запроса службы автообнаружения](#bk_makeautodrequest) на адрес, сопоставленный с папкой в вашем запросе контента.</span><span class="sxs-lookup"><span data-stu-id="a7e39-140">If the mailbox GUID is not the same for all public folders under the public folder root, you need to [Make an Autodiscover request](#bk_makeautodrequest) on the address associated with the folder in your content request.</span></span> 

<span data-ttu-id="a7e39-141"><a name="bk_determineguidews"> </a></span><span class="sxs-lookup"><span data-stu-id="a7e39-141"></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a><span data-ttu-id="a7e39-142">Определите идентификатор GUID почтового ящика общедоступных папок с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="a7e39-142">Determine the GUID of the public folder mailbox by using EWS</span></span>

<span data-ttu-id="a7e39-143">В следующем примере кода показано, как получить значение свойства **PR_REPLICA_LIST** (0x66980102) с помощью веб-служб Exchange [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) операции.</span><span class="sxs-lookup"><span data-stu-id="a7e39-143">The following code example shows how retrieve the value of the **PR_REPLICA_LIST** (0x66980102) property by using the EWS [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="a7e39-144">Для элемента [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) атрибута **PropertyTag** указывается десятичное значение свойства **PR_REPLICA_LIST** (26264), атрибут **PropertyType** задано значение **двоичный**.</span><span class="sxs-lookup"><span data-stu-id="a7e39-144">For the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, the **PropertyTag** attribute is set to the decimal value (26264) of the **PR_REPLICA_LIST** property, and the **PropertyType** attribute is set to **Binary**.</span></span>
  
<span data-ttu-id="a7e39-145">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindFolders** , чтобы [определить GUID почтового ящика общедоступных папок с помощью управляемого интерфейса API веб-служб Exchange](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="a7e39-145">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [determine the GUID of the public folder mailbox by using the EWS Managed API](#bk_determineguidewsma).</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a7e39-146">Сервер отвечает на запрос **FindFolder** [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) сообщение, содержащее значение **PR_REPLICA_LIST** расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="a7e39-146">The server responds to the **FindFolder** request with a [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes the value of the **PR_REPLICA_LIST** extended property.</span></span> <span data-ttu-id="a7e39-147">Обратите внимание, что отображается значение свойства ответа веб-служб Exchange как строку формата base 64 закодированный массив байтов.</span><span class="sxs-lookup"><span data-stu-id="a7e39-147">Note that the value of the property appears on the EWS response as the string format of a base-64 encoded byte array.</span></span> <span data-ttu-id="a7e39-148">Некоторые значения заголовка в ответе сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="a7e39-148">Some header values in the response are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="a7e39-149">Чтобы использовать значение **PR_REPLICA_LIST** возвращается в XML-КОДЕ MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA ==, чтобы определить GUID почтового ящика, значение должны быть преобразованы в идентификатор GUID в формате, аналогичном как значение преобразуется в [Пример кода управляемый API веб-служб Exchange](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="a7e39-149">In order to use the value of the **PR_REPLICA_LIST** returned in the XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, to determine the mailbox GUID, the value must be converted into a GUID in a format similar to how the value is converted in the [EWS Managed API code example](#bk_determineguidewsma).</span></span> <span data-ttu-id="a7e39-150">Идентификатор GUID затем соединяется с именем домена для создания SMTP-адрес, который включен в [запрос автообнаружения](#bk_makeautodrequest).</span><span class="sxs-lookup"><span data-stu-id="a7e39-150">The GUID is then concatenated with the domain name to create an SMTP address, which is included in the [Autodiscover request](#bk_makeautodrequest).</span></span>
  
## <a name="make-an-autodiscover-request"></a><span data-ttu-id="a7e39-151">Для выполнения запроса службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a7e39-151">Make an Autodiscover request</span></span>
<span data-ttu-id="a7e39-152"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="a7e39-152"></span></span>

<span data-ttu-id="a7e39-153">Используйте адрес, возвращенный `GetMailboxGuidAddress` метод, вызываемый службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a7e39-153">Use the address returned by the  `GetMailboxGuidAddress` method to call Autodiscover.</span></span> <span data-ttu-id="a7e39-154">Мы рекомендуем использовать [Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) пример кода для вызова службы автообнаружения, так как он оптимизирует процесса автообнаружения для вас.</span><span class="sxs-lookup"><span data-stu-id="a7e39-154">We recommend that you use the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="a7e39-155">В этом примере код использует аргументы командной строки, указанные в следующей таблице для вызова службы автообнаружения POX для извлечения значения [AutoDiscoverSMTPAddress](http://msdn.microsoft.com/en-us/library/office/dn750991%28v=exchg.150%29.aspx) , связанный с GUID почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a7e39-155">This code sample uses the command-line arguments listed in the following table to call the POX Autodiscover service to retrieve the [AutoDiscoverSMTPAddress](http://msdn.microsoft.com/en-us/library/office/dn750991%28v=exchg.150%29.aspx) value associated with the mailbox GUID.</span></span> 
  
|<span data-ttu-id="a7e39-156">**Argument**</span><span class="sxs-lookup"><span data-stu-id="a7e39-156">**Argument**</span></span>|<span data-ttu-id="a7e39-157">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7e39-157">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7e39-158">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a7e39-158">emailAddress</span></span>  <br/> |<span data-ttu-id="a7e39-159">Адрес, возвращенный `GetMailboxGuidAddress` метода в [Определение GUID почтового ящика общедоступных папок](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="a7e39-159">The address returned by the  `GetMailboxGuidAddress` method in [Determine the GUID of the public folder mailbox](#bk_determineguidewsma).</span></span>  <br/> |
|<span data-ttu-id="a7e39-160">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="a7e39-160">-skipSOAP</span></span>  <br/> |<span data-ttu-id="a7e39-161">Указывает, что запросов автообнаружения POX требуются.</span><span class="sxs-lookup"><span data-stu-id="a7e39-161">Indicates that POX Autodiscover requests are required.</span></span>  <br/> |
|<span data-ttu-id="a7e39-162">-проверкой подлинности на основе authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a7e39-162">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="a7e39-163">Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a7e39-163">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="a7e39-164">Будет предложено ввести пароль пользователя почтового ящика, при выполнении примера.</span><span class="sxs-lookup"><span data-stu-id="a7e39-164">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="a7e39-165">Например аргументы командной строки должна выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="a7e39-165">For example, the command-line arguments should look like this:</span></span>
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="a7e39-166">Где `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` — это адрес, возвращенный методом **GetMailboxGuidAddress** и `sonyaf@contoso.com` — пользователь, почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="a7e39-166">Where `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` is the address returned by the **GetMailboxGuidAddress** method, and `sonyaf@contoso.com` is the mailbox user.</span></span> 
  
<span data-ttu-id="a7e39-167">При выполнении **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, последний ответ автообнаружения должен быть успешные и включают все пользовательские параметры, связанные с GUID почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a7e39-167">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="a7e39-168">Сохранить **AutoDiscoverSMTPAddress** пользователя, задание локально, как она будет использоваться на следующем этапе.</span><span class="sxs-lookup"><span data-stu-id="a7e39-168">Save the **AutoDiscoverSMTPAddress** user setting locally, as you'll use that in the next step.</span></span> 
  
<span data-ttu-id="a7e39-169">Кроме того Если вы не хотите использовать **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, вы получаете пользователя **AutoDiscoverSMTPAddress** параметру, [создав список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и затем Отправка следующие Запрос автообнаружения POX для каждого URL-адреса до получения успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="a7e39-169">Alternatively, if you do not want to use **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **AutoDiscoverSMTPAddress** user setting by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="a7e39-170">Дополнительные сведения о процессе автообнаружения можно [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создать список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="a7e39-170">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="a7e39-171">Задайте значения заголовков X AnchorMailbox и X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a7e39-171">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="a7e39-172"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="a7e39-172"></span></span>

<span data-ttu-id="a7e39-173">С использованием значения для **AutoDiscoverSMTPAddress** , полученные в [выполнения запроса службы автообнаружения](#bk_makeautodrequest), задайте значения заголовков **X AnchorMailbox** и **X-PublicFolderMailbox** в вашем запросе контента общей папки.</span><span class="sxs-lookup"><span data-stu-id="a7e39-173">Using the value for the **AutoDiscoverSMTPAddress** acquired in [Make an Autodiscover request](#bk_makeautodrequest), set the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="a7e39-174">Например учитывая AutoDiscoverSMTPAddress NewPublicFolder@contoso.com, включают следующие заголовки при вызове следующих методов или операции.</span><span class="sxs-lookup"><span data-stu-id="a7e39-174">For example, given an AutoDiscoverSMTPAddress of NewPublicFolder@contoso.com, include the following headers when making calls to the following methods or operations.</span></span>
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

<span data-ttu-id="a7e39-175">**Вызовы общих папок, которые требуют X AncorMailbox и X-PublicFolder заголовков**</span><span class="sxs-lookup"><span data-stu-id="a7e39-175">**Public folder calls that require the X-AncorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="a7e39-176">**Методы управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="a7e39-176">**EWS Managed API methods**</span></span>|<span data-ttu-id="a7e39-177">**Операции EWS**</span><span class="sxs-lookup"><span data-stu-id="a7e39-177">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7e39-178">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="a7e39-178">Item.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-179">Item.Update</span><span class="sxs-lookup"><span data-stu-id="a7e39-179">Item.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-180">Item.Copy</span><span class="sxs-lookup"><span data-stu-id="a7e39-180">Item.Copy</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-181">Item.Move</span><span class="sxs-lookup"><span data-stu-id="a7e39-181">Item.Move</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-182">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="a7e39-182">Item.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-183">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="a7e39-183">Folder.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a7e39-184">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="a7e39-184">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a7e39-185">CreateItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-185">CreateItem</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-186">GetItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-186">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-187">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-187">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-188">CopyItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-188">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-189">MoveItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-189">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-190">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-190">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> [<span data-ttu-id="a7e39-191">GetFolder</span><span class="sxs-lookup"><span data-stu-id="a7e39-191">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="a7e39-192">FindItem</span><span class="sxs-lookup"><span data-stu-id="a7e39-192">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="a7e39-193">Чтобы добавить эти заголовки с помощью управляемого интерфейса API веб-служб Exchange, используйте метод [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a7e39-193">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

<span data-ttu-id="a7e39-194">В следующем коде показан запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) с заголовка **X-AnchorMailbox** и **X PublicFolderMailbox** , значения, полученные на примерах в этой статье.</span><span class="sxs-lookup"><span data-stu-id="a7e39-194">The following code shows a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a7e39-195">См. также</span><span class="sxs-lookup"><span data-stu-id="a7e39-195">See also</span></span>

- [<span data-ttu-id="a7e39-196">Общих папок в Exchange доступ с EWS</span><span class="sxs-lookup"><span data-stu-id="a7e39-196">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="a7e39-197">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="a7e39-197">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="a7e39-198">Создание списка конечных точек автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a7e39-198">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [<span data-ttu-id="a7e39-199">Получить параметры пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a7e39-199">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

