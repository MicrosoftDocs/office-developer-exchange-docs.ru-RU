---
title: Импорт элементов с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: bc874c667c31beb4e59a305626247488cb1a1781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527987"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="25b62-103">Импорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="25b62-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="25b62-104">Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b62-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="25b62-105">Многие системы содержат встречи, сообщения электронной почты, контакты и задачи, а также могут импортировать эти элементы в Exchange несколькими различными способами.</span><span class="sxs-lookup"><span data-stu-id="25b62-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="25b62-106">Импорт элементов в Exchange выполняется просто, если для этих элементов не поддерживаются отношения почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="25b62-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="25b62-107">Для создания элементов в почтовом ящике Exchange можно использовать метод [Item. Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) управляемый API EWS или операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="25b62-107">You can use the [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="25b62-108">Простой подход не поддерживает все сценарии, однако. Например:</span><span class="sxs-lookup"><span data-stu-id="25b62-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="25b62-109">Вы не можете поддерживать связь между организаторов и участниками при импорте встреч с участниками (собраниями).</span><span class="sxs-lookup"><span data-stu-id="25b62-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="25b62-110">Это означает, что организатору собрания потребуется повторить отправку приглашений на собрания для участников, чтобы установить связь между организатором и участниками.</span><span class="sxs-lookup"><span data-stu-id="25b62-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="25b62-111">Если встреча была импортирована в календарь участника, встреча не будет связана с встречей организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="25b62-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="25b62-112">Участникам необходимо принять приглашение на собрание, отправленное из организатора, чтобы восстановить связь с организатором.</span><span class="sxs-lookup"><span data-stu-id="25b62-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="25b62-113">Сведения о уполномоченные не сохраняются при импорте назначенных задач.</span><span class="sxs-lookup"><span data-stu-id="25b62-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="25b62-114">Все параметры импорта можно использовать для пакетного импорта элементов в Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b62-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="25b62-115">Использование управляемого API EWS или типов элементов EWS для импорта элемента</span><span class="sxs-lookup"><span data-stu-id="25b62-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="25b62-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="25b62-116"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="25b62-117">Вы можете использовать управляемый API EWS или EWS для импорта электронных сообщений, контактов, встреч или задач из других систем.</span><span class="sxs-lookup"><span data-stu-id="25b62-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="25b62-118">Просто присвойте [свойствам](properties-and-extended-properties-in-ews-in-exchange.md) исходного формата любой из следующих объектов в зависимости от того, что вы импортируете.</span><span class="sxs-lookup"><span data-stu-id="25b62-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="25b62-119">**Таблица 1. Объекты управляемого API EWS и элементы EWS**</span><span class="sxs-lookup"><span data-stu-id="25b62-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="25b62-120">**Объект управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="25b62-120">**EWS Managed API object**</span></span>|<span data-ttu-id="25b62-121">**Элемент EWS**</span><span class="sxs-lookup"><span data-stu-id="25b62-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25b62-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="25b62-122">EmailMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25b62-123">Сообщение</span><span class="sxs-lookup"><span data-stu-id="25b62-123">Message</span></span>](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25b62-124">[контакт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx);</span><span class="sxs-lookup"><span data-stu-id="25b62-124">[Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="25b62-125">[контакт](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx);</span><span class="sxs-lookup"><span data-stu-id="25b62-125">[Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx)</span></span> <br/> |
|[<span data-ttu-id="25b62-126">Встреча</span><span class="sxs-lookup"><span data-stu-id="25b62-126">Appointment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25b62-127">календаритем</span><span class="sxs-lookup"><span data-stu-id="25b62-127">CalendarItem</span></span>](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="25b62-128">Task</span><span class="sxs-lookup"><span data-stu-id="25b62-128">Task</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25b62-129">Task</span><span class="sxs-lookup"><span data-stu-id="25b62-129">Task</span></span>](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="25b62-130">Используйте метод [Item. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) Managed API или операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для выполнения импорта элементов.</span><span class="sxs-lookup"><span data-stu-id="25b62-130">Use the [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="25b62-131">Этот подход рекомендуется при импорте элементов из других систем, так как вы контролируете, какие свойства будут импортированы.</span><span class="sxs-lookup"><span data-stu-id="25b62-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="25b62-132">Дополнительные сведения о том, как задать свойства элементов и затем сохранить элемент, можно узнать в статье [Создание элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) или [Создание элемента с помощью EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="25b62-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="25b62-133">Импорт элементов с полными качествами</span><span class="sxs-lookup"><span data-stu-id="25b62-133">Import items with full fidelity</span></span>
<span data-ttu-id="25b62-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="25b62-134"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="25b62-135">Вы можете использовать операцию [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS для отправки элемента в качестве потока данных.</span><span class="sxs-lookup"><span data-stu-id="25b62-135">You can use the [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="25b62-136">Это представление потока данных элемента должно поступать из результатов вызова операции [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="25b62-136">This data stream representation of an item has to come from the results of an [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="25b62-137">Так как управляемый API EWS не реализует операцию **UploadItems** , если вы используете управляемый API EWS, вам потребуется написать процедуру для отправки веб-запросов.</span><span class="sxs-lookup"><span data-stu-id="25b62-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="25b62-138">Это самый простой способ импортировать элементы, экспортированные с другого сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="25b62-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="25b62-139">В следующем примере идентификаторы и содержимое элемента **данных** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25b62-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId  Id="AAMkADEzOTE7kV0AAA=" ChangeKey="AQAAAA=="/>
          <t:Data>AQAAAAgAAAAAAQAAAAADABZADQASDkANABMO</t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **UploadItems** с помощью элемента [уплоадитемсреспонсе](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) , который содержит значение элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) с **ошибкой**, что указывает на то, что элемент был успешно отправлен. <span data-ttu-id="25b62-141">Ответ также включает идентификатор элемента отправленного элемента.</span><span class="sxs-lookup"><span data-stu-id="25b62-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="25b62-142">Использование потока MIME для импорта из распространенных форматов файлов</span><span class="sxs-lookup"><span data-stu-id="25b62-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="25b62-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="25b62-143"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="25b62-144">В веб-службах EWS можно импортировать файлы EML (EML) и iCal (ICS).</span><span class="sxs-lookup"><span data-stu-id="25b62-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="25b62-145">Вы хотите протестировать содержимое MIME, чтобы увидеть, как средство синтаксического анализа MIME Exchange обрабатывает содержимое потока MIME.</span><span class="sxs-lookup"><span data-stu-id="25b62-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="25b62-146">Хотя использование потока MIME удобно, [для импорта элемента лучше использовать управляемый API EWS или типы элементов EWS](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="25b62-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="25b62-147">Ниже приведен пример [импорта визитной карточки](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="25b62-147">Here's an example of how to [import a vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="25b62-148">Использование управляемого API EWS для импорта электронной почты из EML-файла с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="25b62-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="25b62-149">В приведенном ниже примере показано, как задать свойство [сохранитьmimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) с содержимым файла EML и затем импортировать его в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="25b62-149">The following example shows how to set the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="25b62-150">В этом примере также показано, как задать расширенное свойство [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) для импортированного электронного сообщения, чтобы оно не отображалось в почтовом ящике как элемент черновика.</span><span class="sxs-lookup"><span data-stu-id="25b62-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="25b62-151">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b62-151">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void UploadMIMEEmail(ExchangeService service)
{
    EmailMessage email = new EmailMessage(service);
    
    string emlFileName = @"C:\import\email.eml";
    using (FileStream fs = new FileStream(emlFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .eml file to the MimeContent property.
        email.MimeContent = new MimeContent("UTF-8", bytes);
    }
    
    // Indicate that this email is not a draft. Otherwise, the email will appear as a 
    // draft to clients.
    ExtendedPropertyDefinition PR_MESSAGE_FLAGS_msgflag_read = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
    email.SetExtendedProperty(PR_MESSAGE_FLAGS_msgflag_read, 1);
    // This results in a CreateItem call to EWS. The email will be saved in the Inbox folder.
    email.Save(WellKnownFolderName.Inbox);
}
```

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="25b62-152">Использование управляемого API EWS для импорта встречи из файла iCal с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="25b62-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="25b62-153">Вы можете импортировать простые встречи в виде файлов iCalendar с помощью потока MIME.</span><span class="sxs-lookup"><span data-stu-id="25b62-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="25b62-154">Вы не можете импортировать собрания, которые являются встречами с участниками, так как отношение между собраниями организаторов и участниками должно быть задано в составе рабочего процесса [календаря Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="25b62-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="25b62-155">Участники не могут быть захвачены в потоке MIME.</span><span class="sxs-lookup"><span data-stu-id="25b62-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="25b62-156">В приведенном ниже примере кода показано, как импортировать простой файл ICS в почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="25b62-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
```cs
private static void UploadMIMEAppointment(ExchangeService service)
{
    Appointment appointment = new Appointment(service);
    string iCalFileName = @"C:\import\appointment.ics";
    using (FileStream fs = new FileStream(iCalFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .ics file to the MimeContent property.
        appointment.MimeContent = new MimeContent("UTF-8", bytes);
    }
    // This results in a CreateItem call to EWS. 
    appointment.Save(WellKnownFolderName.Calendar);
}
```

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="25b62-157">Использование EWS для импорта элемента с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="25b62-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="25b62-158">Вы можете использовать операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для импорта элементов EML и iCal с помощью потока MIME.</span><span class="sxs-lookup"><span data-stu-id="25b62-158">You can use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body >
    <m:CreateItem>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </m:SavedItemFolderId> 
        <m:Items>
        <t:Message>
          <t:MimeContent CharacterSet="UTF-8">
            <!-- Insert MIME content here-->
          </t:MimeContent>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="25b62-159">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="25b62-159">Next steps</span></span>
<span data-ttu-id="25b62-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="25b62-160"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="25b62-161">После импорта элементов в почтовый ящик может потребоваться [создать настраиваемую папку для хранения импортируемых элементов](how-to-work-with-folders-by-using-ews-in-exchange.md)или [синхронизировать элементы клиента и почтового ящика](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="25b62-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="25b62-162">См. также</span><span class="sxs-lookup"><span data-stu-id="25b62-162">See also</span></span>


- [<span data-ttu-id="25b62-163">Экспорт и импорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="25b62-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25b62-164">Экспорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="25b62-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25b62-165">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="25b62-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="25b62-166">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="25b62-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

