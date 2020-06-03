---
title: Операция AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Поиск сведений о AddImContactToGroupной операции EWS.
ms.openlocfilehash: a69ee0b355e78e1249383cab612a75bcda8d9e8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458413"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="f6708-103">Операция AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="f6708-104">Поиск сведений о **AddImContactToGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="f6708-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="f6708-105">**AddImContactToGroup** веб-служб Exchange (EWS) добавляет в группу существующего контакта обмена мгновенными сообщениями (IM).</span><span class="sxs-lookup"><span data-stu-id="f6708-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="f6708-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f6708-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="f6708-107">Использование операции AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="f6708-108">Операция **AddImContactToGroup** может принимать только контакты для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f6708-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="f6708-109">Если вы хотите добавить новый контакт для обмена мгновенными сообщениями в единое хранилище контактов, используйте операцию [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f6708-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="f6708-110">Операция **AddImContactToGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="f6708-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="f6708-111">**Таблица 1. Заголовки SOAP операции AddImContactToGroup**</span><span class="sxs-lookup"><span data-stu-id="f6708-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="f6708-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="f6708-112">**Header name**</span></span>|<span data-ttu-id="f6708-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6708-113">**Element**</span></span>|<span data-ttu-id="f6708-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6708-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f6708-115">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="f6708-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="f6708-116">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="f6708-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f6708-117">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="f6708-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="f6708-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="f6708-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f6708-119">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="f6708-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="f6708-120">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="f6708-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f6708-121">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="f6708-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="f6708-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="f6708-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f6708-123">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="f6708-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f6708-124">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="f6708-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f6708-125">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="f6708-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f6708-126">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="f6708-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f6708-127">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="f6708-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f6708-128">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="f6708-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f6708-129">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="f6708-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f6708-130">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="f6708-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="f6708-131">Пример запроса операции AddImContactToGroup: Добавление существующего контакта для обмена мгновенными сообщениями в группу обмена мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="f6708-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="f6708-132">В приведенном ниже примере запроса операции **AddImContactToGroup** показано, как добавить существующий обмен мгновенными сообщениями в группу обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f6708-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f6708-133">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f6708-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f6708-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="f6708-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="f6708-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="f6708-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="f6708-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="f6708-137">Успешный отклик операции AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="f6708-138">В следующем примере показан успешный ответ на запрос операции **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="f6708-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="f6708-139">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f6708-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f6708-140">аддимконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="f6708-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="f6708-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f6708-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="f6708-142">Ответ об ошибке Ерроринвалидимконтактид операции AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="f6708-143">В следующем примере показан ответ об ошибке для запроса операции **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="f6708-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="f6708-144">При попытке добавить контакт, который не является контактом для обмена мгновенными сообщениями, возникает следующий ответ об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f6708-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="f6708-145">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f6708-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f6708-146">аддимконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="f6708-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="f6708-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f6708-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f6708-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f6708-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f6708-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="f6708-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="f6708-150">См. также</span><span class="sxs-lookup"><span data-stu-id="f6708-150">See also</span></span>

- [<span data-ttu-id="f6708-151">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="f6708-152">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="f6708-153">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="f6708-154">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="f6708-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="f6708-155">Операция GetImItemList</span><span class="sxs-lookup"><span data-stu-id="f6708-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="f6708-156">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="f6708-156">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

