---
title: глобаликониндекс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d28ed70-4cfe-46e4-8d15-593c6e355bcf
description: Элемент Глобаликониндекс определяет глобальный индекс значков для всех элементов в беседе.
ms.openlocfilehash: 9900a80136a1a7eaae4634afd31568679f6dba1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459463"
---
# <a name="globaliconindex"></a>глобаликониндекс

Элемент **глобаликониндекс** определяет глобальный индекс значков для всех элементов в беседе. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MaillrmForwarded | MaillrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **икониндекстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[Беседа (конверсатионтипе)](conversation-conversationtype.md)  |  [Элемент](item.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [Календаритем](calendaritem.md)  |  [Элемент](postitem.md)  |  i [Task (задача](task.md) )
  
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные текстовые значения для элемента **глобаликониндекс** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|||
|По умолчанию  <br/> |Задает значок по умолчанию.  <br/> |
|PostItem  <br/> |Задает значок элемента POST.  <br/> |
|маилреад  <br/> |Указывает значок чтения почты.  <br/> |
|маилунреад  <br/> |Указывает значок непрочтенной почты.  <br/> |
|маилреплиед  <br/> |Указывает значок "ответ на сообщение".  <br/> |
|маилфорвардед  <br/> |Указывает значок переадресованной почты.  <br/> |
|маиленкриптед  <br/> |Указывает значок зашифрованной почты.  <br/> |
|маилсмимесигнед  <br/> |Указывает значок подписанного почтового расширения для безопасного или многоцелевого расширения почты в Интернете (S/MIME).  <br/> |
|маиленкриптедреплиед  <br/> |Указывает зашифрованный значок, на который отправлен ответ.  <br/> |
|маилсмимесигнедреплиед  <br/> |Указывает значок почтового ящика с подписанным сообщением S/MIME.  <br/> |
|маиленкриптедфорвардед  <br/> |Указывает значок зашифрованной переадресованной почты.  <br/> |
|маилсмимесигнедфорвардед  <br/> |Указывает значок переадресованного почтового ящика с подписью S/MIME.  <br/> |
|маиленкриптедреад  <br/> |Задает зашифрованный значок чтения почты.  <br/> |
|маилсмимесигнедреад  <br/> |Указывает подписанный значок чтения почты S/MIME.  <br/> |
|маилирм  <br/> |Указывает значок защищенной службы управления правами на доступ к данным (IRM).  <br/> |
|маилирмфорвардед  <br/> |Указывает значок переадресованной почты с защитой IRM.  <br/> |
|маилирмреплиед  <br/> |Указывает значок почты, защищенный с помощью службы управления правами на доступ к данным.  <br/> |
|смссубмиттед  <br/> |Задает значок для почты, отправленной для маршрутизации в службе коротких сообщений (SMS).  <br/> |
|смсраутедтоделиверипоинт  <br/> |Задает значок маршрутизации SMS для внешней точки доставки.  <br/> |
|смсраутедтоекстерналмессагингсистем  <br/> |Задает значок маршрутизации SMS для внешней системы обмена сообщениями.  <br/> |
|смсделиверед  <br/> |Указывает значок доставленной почты SMS.  <br/> |
|аутлукдефаултфорконтактс  <br/> |Задает значок по умолчанию для контактов.  <br/> |
|AppointmentItem  <br/> |Задает значок элемента встречи.  <br/> |
|аппоинтментрекур  <br/> |Задает значок повторяющейся встречи.  <br/> |
|аппоинтментмит  <br/> |Указывает значок собрания.  <br/> |
|аппоинтментмитрекур  <br/> |Задает значок повторяющегося собрания.  <br/> |
|аппоинтментмитни  <br/> |Задает значок ответа на приглашение на собрание.  <br/> |
|аппоинтментмитес  <br/> |Указывает значок принятия приглашения на собрание.  <br/> |
|аппоинтментмитно  <br/> |Указывает значок "собрание отклонено".  <br/> |
|аппоинтментмитмайбе  <br/> |Задает значок, который может отреагировать на собрание.  <br/> |
|аппоинтментмитканцел  <br/> |Указывает значок отмены собрания.  <br/> |
|аппоинтментмитинфо  <br/> |Указывает значок сведений о собрании.  <br/> |
|TaskItem  <br/> |Задает значок элемента задачи.  <br/> |
|таскрекур  <br/> |Задает значок повторяющейся задачи.  <br/> |
|тасковнед  <br/> |Указывает значок владельца задачи.  <br/> |
|таскделегатед  <br/> |Задает делегированный значок задачи.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

