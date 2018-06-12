---
title: Операция GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: Операция GetDelegate Получение параметров делегат для указанного почтового ящика.
ms.openlocfilehash: bd1a0add54ee5fd1c23b4ba09a921a9061afa394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762742"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="96de7-103">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="96de7-103">GetDelegate operation</span></span>

<span data-ttu-id="96de7-104">Операция **GetDelegate** Получение параметров делегат для указанного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="96de7-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="96de7-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="96de7-105">SOAP Headers</span></span>

<span data-ttu-id="96de7-106">Операция **GetDelegate** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="96de7-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="96de7-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="96de7-107">**Header**</span></span>|<span data-ttu-id="96de7-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="96de7-108">**Element**</span></span>|<span data-ttu-id="96de7-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96de7-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="96de7-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="96de7-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="96de7-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="96de7-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="96de7-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="96de7-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="96de7-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="96de7-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="96de7-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="96de7-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="96de7-115">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="96de7-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="96de7-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="96de7-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="96de7-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="96de7-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="96de7-118">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="96de7-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="96de7-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="96de7-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="96de7-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="96de7-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="96de7-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="96de7-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="96de7-122">Пример запроса GetDelegate</span><span class="sxs-lookup"><span data-stu-id="96de7-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="96de7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="96de7-123">Description</span></span>

<span data-ttu-id="96de7-124">В следующем примере кода показано, как получить параметры делегат для всех делегатов, заданные для почтового ящика пользователя user3.</span><span class="sxs-lookup"><span data-stu-id="96de7-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="96de7-125">В ответе возвращаются все разрешения для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="96de7-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="96de7-126">Программа</span><span class="sxs-lookup"><span data-stu-id="96de7-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="96de7-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="96de7-127">Comments</span></span>

<span data-ttu-id="96de7-128">Элемент [UserId](userid.md) можно использовать для определения отдельных пользователей вместо возврата всех пользователей, имеющих делегирование прав доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="96de7-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="96de7-129">Веб-служб Exchange (EWS) не поддерживает управление представителями группы.</span><span class="sxs-lookup"><span data-stu-id="96de7-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="96de7-130">Веб-служб Exchange возвратит ошибку, если операция **GetDelegate** вызывается для участником с представителем группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="96de7-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="96de7-131">Пример ответа GetDelegate</span><span class="sxs-lookup"><span data-stu-id="96de7-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="96de7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96de7-132">Description</span></span>

<span data-ttu-id="96de7-133">В следующем примере ответа **GetDelegate** показано успешного ответа на запрос **GetDelegate** .</span><span class="sxs-lookup"><span data-stu-id="96de7-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="96de7-134">Ответ содержит сведения о разрешениях доступа делегата, были доставлены ли делегированный пользователь может просматривать личные элементы ли представитель получает копии приглашений на собрания сообщений и которому собрания запросов.</span><span class="sxs-lookup"><span data-stu-id="96de7-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="96de7-135">Программа</span><span class="sxs-lookup"><span data-stu-id="96de7-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:GetDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="96de7-136">См. также</span><span class="sxs-lookup"><span data-stu-id="96de7-136">See also</span></span>



- [<span data-ttu-id="96de7-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="96de7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

