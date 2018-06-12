---
title: Создание группы контактов с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Узнайте, как создать группу контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760992"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="15888-103">Создание группы контактов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="15888-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="15888-104">Узнайте, как создать группу контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="15888-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="15888-105">Можно создать группу контактов, являющийся частной [группы рассылки](distribution-groups-and-ews-in-exchange.md), с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="15888-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="15888-106">Создание группы контактов, использовать методы в классе управляемый API EWS [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) или с помощью операции [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="15888-106">To create contact groups, use the methods in the [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="15888-107">Обратите внимание на то, что нельзя использовать управляемый API EWS или веб-служб Exchange для создания универсальная группа рассылки или группу безопасности.</span><span class="sxs-lookup"><span data-stu-id="15888-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="15888-108">Чтобы создать универсальная группа рассылки или группу безопасности, можно использовать [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[командлет командной консоли Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="15888-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="15888-109">Создание группы контактов с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="15888-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="15888-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="15888-110"></span></span>

<span data-ttu-id="15888-111">Чтобы создать группу контактов, достаточно несколько видов информации: имя группы и элементы для добавления в группу.</span><span class="sxs-lookup"><span data-stu-id="15888-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="15888-112">Приведенный ниже показано, как создать простой группы контактов, содержащий несколько членов группы.</span><span class="sxs-lookup"><span data-stu-id="15888-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
```cs
// Create a new contact group object.
ContactGroup myContactGroup = new ContactGroup(service);
// Give the group a name.
myContactGroup.DisplayName = "My Contact Group";
// Add some members to the group.
myContactGroup.Members.Add(new GroupMember("sadie@contoso.com"));
myContactGroup.Members.Add(new GroupMember("alfred@contoso.com"));
// Save the group.
myContactGroup.Save();

```

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="15888-113">Создание группы контактов с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="15888-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="15888-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="15888-114"></span></span>

<span data-ttu-id="15888-115">Выполнение может занять несколько дополнительные строки кода, но можно создать группу контактов с помощью операции [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="15888-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="15888-116">В следующем примере запрос XML показано, как создать группу контактов.</span><span class="sxs-lookup"><span data-stu-id="15888-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="15888-117">Это также запроса XML, который отправляется, когда [использовать управляемый API веб-служб Exchange для создания группы контактов](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="15888-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

<span data-ttu-id="15888-118">Ниже приведен пример успешного ответа XML для запроса.</span><span class="sxs-lookup"><span data-stu-id="15888-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="15888-119">Обратите внимание, что возвращаемые значения включают идентификатор элемента для новой группы контактов и изменить ключ, можно использовать в другой код для изменения группы контактов или разверните группу, чтобы просмотреть список членов.</span><span class="sxs-lookup"><span data-stu-id="15888-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="15888-120">Идентификатор элемента сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="15888-120">The item ID is shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a><span data-ttu-id="15888-121">См. также</span><span class="sxs-lookup"><span data-stu-id="15888-121">See also</span></span>


- [<span data-ttu-id="15888-122">Группы рассылки и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="15888-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="15888-123">Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="15888-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

