---
title: митингмессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingMessage
api_type:
- schema
ms.assetid: c95956a8-7505-44b4-bea4-11d1f5182796
description: Элемент Митингмессаже представляет собрание в хранилище Exchange.
ms.openlocfilehash: fee615a1da117e5df03cd5ce8576bd66d7e89a4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468385"
---
# <a name="meetingmessage"></a>митингмессаже

Элемент **митингмессаже** представляет собрание в хранилище Exchange. 
  
```xml
<MeetingMessage>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</MeetingMessage>
```

 **митингмессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сохранитьmimecontent](mimecontent.md) <br/> |Содержит собственный поток MIME объекта, представленный в формате base64Binary.  <br/> |
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения для элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объектов ответа. Тема может иметь не более 255 символов.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Содержит статус чувствительности элемента.  <br/> |
|[Body](body.md) <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер элемента в байтах. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, определяющих, к каким категориям принадлежит элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[инреплито](inreplyto.md) <br/> |Представляет идентификатор элемента, который является ответом на этот элемент.  <br/> |
|[Отправлено](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.  <br/> |
|[Черновик](isdraft.md) <br/> |Указывает, был ли элемент еще не отправлен.  <br/> |
|[исфромме](isfromme.md) <br/> |Указывает, отправляет ли пользователь элемент.  <br/> |
|[исресенд](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[исунмодифиед](isunmodified.md) <br/> |Указывает, был ли изменен элемент.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элементе почтового ящика.  <br/> |
|[датетимесент](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания определенного элемента в почтовом ящике.  <br/> |
|[респонсеобжектс](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.  <br/> |
|[реминдердуеби](reminderdueby.md) <br/> |Представляет дату и время возникновения события. Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[реминдериссет](reminderisset.md) <br/> |Указывает, задано ли напоминание для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события при отображении напоминания.  <br/> |
|[дисплайкк](displaycc.md) <br/> |Представляет отображаемую строку, используемую для содержимого поля "копия". Это объединенная строка всех отображаемых имен получателей копии.  <br/> |
|[дисплайто](displayto.md) <br/> |Представляет отображаемую строку, используемую для содержимого поля "Кому". Это объединенная строка для отображаемых имен получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет язык и региональные параметры для определенного элемента в почтовом ящике.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправителя элемента.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит набор получателей сообщения.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.  <br/> |
|[исреадрецеиптрекуестед](isreadreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента уведомление о прочтении.  <br/> |
|[исделиверирецеиптрекуестед](isdeliveryreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента уведомление о доставке.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичный код, представляющий поток, к которому относится сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет адрес получателя, от которого было отправлено сообщение.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения Интернета для элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли Прочитано сообщение.  <br/> |
|[исреспонсерекуестед](isresponserequested.md) <br/> |Указывает, запрашивается ли ответ на сообщение электронной почты.  <br/> |
|[References](references.md) <br/> |Представляет заголовок Usenet, используемый для сопоставления ответов с их исходными сообщениями.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет набор адресов, в который отправляются ответы.  <br/> |
|[ассоЦиатедкалендаритемид](associatedcalendaritemid.md) <br/> |Представляет элемент календаря, связанный с объектом [митингмессаже](meetingmessage.md).  <br/> |
|[Isdelegated для](isdelegated.md) <br/> |Указывает, было ли собрание обработано с помощью учетной записи с делегированным доступом.  <br/> |
|[IsOutOfDate](isoutofdate.md) <br/> |Указывает, является ли сообщение о собрании устаревшим.  <br/> |
|[хасбинпроцессед](hasbeenprocessed.md) <br/> |Указывает, был ли обработан элемент сообщения о собрании.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип ответа получателя, полученный для собрания.  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[ластмодифиеднаме](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя для изменения элемента.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[Связанный](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[вебклиентреадформкуеристринг](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[вебклиентедитформкуеристринг](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.  <br/> |
|[UID](uid.md) <br/> |Определяет элемент календаря.  <br/> |
|[рекурренцеид](recurrenceid.md) <br/> |Используется для идентификации определенного экземпляра повторяющегося элемента календаря.  <br/> |
|[датетиместамп](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аджацентмитингс](adjacentmeetings.md) <br/> |Описывает все элементы календаря, смежные с временем собрания.  <br/> |
|[аппендтоитемфиелд](appendtoitemfield.md) <br/> |Определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуют с временем собрания.  <br/> |
|[Create (Итемсинк)](create-itemsync.md) <br/> |Определяет один элемент, который необходимо создать в локальном хранилище клиента.  <br/> |
|[Обновление (Итемсинк)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определенной элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[сетитемфиелд](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

