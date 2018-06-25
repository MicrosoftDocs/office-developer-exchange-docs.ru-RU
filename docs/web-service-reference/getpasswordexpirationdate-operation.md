---
title: Операция GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: Операция GetPasswordExpirationDate предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762874"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="7eb11-103">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7eb11-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="7eb11-104">Операция **GetPasswordExpirationDate** предоставляет срок действия пароля учетной записи электронной почты для текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="7eb11-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="7eb11-105">Эта операция была введена в пакете обновления 1 (SP1) для Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="7eb11-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="7eb11-106">Заголовки SOAP GetPasswordExpirationDate операции</span><span class="sxs-lookup"><span data-stu-id="7eb11-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="7eb11-107">Операция **GetPasswordExpirationDate** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7eb11-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7eb11-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="7eb11-108">**Header**</span></span>|<span data-ttu-id="7eb11-109">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7eb11-109">**Element**</span></span>|<span data-ttu-id="7eb11-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7eb11-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7eb11-111">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="7eb11-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="7eb11-112">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7eb11-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="7eb11-113">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="7eb11-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="7eb11-114">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="7eb11-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7eb11-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7eb11-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7eb11-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7eb11-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7eb11-117">Определяет схему для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="7eb11-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="7eb11-118">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="7eb11-118">This is applicable to a request.</span></span> <span data-ttu-id="7eb11-119">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="7eb11-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="7eb11-120">Пример запроса GetPasswordExpirationDate операции</span><span class="sxs-lookup"><span data-stu-id="7eb11-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="7eb11-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7eb11-121">Description</span></span>

<span data-ttu-id="7eb11-122">В следующем примере запрос операции **GetPasswordExpirationDate** показано, как получить срок действия пароля для учетной записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7eb11-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7eb11-123">Программа</span><span class="sxs-lookup"><span data-stu-id="7eb11-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="7eb11-124">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="7eb11-124">Request elements</span></span>

<span data-ttu-id="7eb11-125">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7eb11-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7eb11-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7eb11-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="7eb11-127">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7eb11-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="7eb11-128">Успешные операции ответа GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7eb11-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="7eb11-129">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7eb11-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7eb11-130">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="7eb11-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="7eb11-131">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7eb11-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

