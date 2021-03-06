---
title: Передача прав доступа и EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 240d1776-7adc-46cd-9099-88ffeba0a8aa
description: Узнайте, как использовать управляемый API EWS и EWS в Exchange для предоставления представителю доступа к почтовым ящикам пользователей.
localization_priority: Priority
ms.openlocfilehash: 4223d625213a3f71726ec5b8d3f09f9e2e7e7e51
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528456"
---
# <a name="delegate-access-and-ews-in-exchange"></a>Передача прав доступа и EWS в Exchange

Узнайте, как использовать управляемый API EWS и EWS в Exchange для предоставления представителю доступа к почтовым ящикам пользователей.
  
Вы можете разрешить пользователям доступ к почтовым ящикам других пользователей одним из трех способов: 
  
- Путем добавления делегатов и указания разрешений для каждого делегата.
    
- Путем непосредственного изменения разрешений на доступ к папке.
    
- С помощью олицетворения.
    
Разрешения на делегирование и папки лучше всего предоставить доступ только нескольким пользователям, так как необходимо добавлять разрешения по отдельности для каждого почтового ящика. Олицетворение является лучшим выбором при работе с количествами почтовых ящиков, так как для доступа к каждому почтовому ящику в базе данных можно легко включить одну учетную запись службы. На рисунке 1 показаны некоторые различия между типами доступа.
  
**Рис. 1. Способы доступа к почтовым ящикам других пользователей**

![Схема, на которой показаны типы доступа к почтовому ящику, связь между владельцами почтовых ящиков и делегатом для каждого типа, а также тип разрешения. Отправка от лица разрешений для делегирования и разрешений папок. Отправка как разрешений для олицетворения.](media/Ex15_Delegate_Overview.png)
  
При отправке сообщений или планировании собраний делегатам могут быть предоставлены разрешения "Отправить от имени", поэтому получатель электронной почты или приглашения на собрание, отправленные представителем, увидят сообщение " *делегат* от имени *владельца почтового ящика* " при получении им доступа к электронной почте или приглашению на собрание в Outlook. Включение текста "Отправить от имени" является подробным описанием реализации клиента и может создаваться с использованием значений "от" и "sender". Значение "от" указывает владельца почтового ящика, а значение "sender" указывает представителя, который отправил почту. Если учетная запись службы, с помощью которой выполняется олицетворение пользователя отправляет сообщение электронной почты или планирует собрание для владельца почтового ящика, сообщение "отправляется как" владельца почтового ящика. У получателя нет способа узнать, что почта была отправлена учетной записью службы. Пользователи, которым предоставлены разрешения на доступ к папкам, а не представителю, не могут "Отправить как" или "Отправить от имени" владельца почтового ящика. У них есть доступ к папкам почтового ящика, и они могут создавать элементы в папках, но не могут отправлять элементы. 
  
Когда нужно изменять разрешения для папки напрямую? Как правило, если вы хотите предоставить пользователю доступ к папке, но не хотите предоставлять пользователю разрешения "Отправить от имени", если требования к разрешениям не соответствуют значениям перечисления [делегатефолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) EWS Managed API или значениям элементов [пермиссионлевел](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) EWS, или если вы хотите предоставить пользователю доступ к одной пользовательской папке. 
  
Если вам нужно изменить разрешения для папки, чтобы ее можно было использовать, и не нужно добавлять делегата (то есть вам не требуется разрешение "Отправить от имени"), ознакомьтесь с [разрешениями Set Folders for другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md). 

Обратите внимание, что вы также можете настроить доступ представителя с помощью [Outlook](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx) или [PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) . 

  
## <a name="how-does-delegate-access-work"></a>Как работает делегированный доступ?

Делегированный доступ позволяет пользователям получать доступ к некоторым или всем папкам владельца почтового ящика и выполнять действия от имени владельца почтового ящика. Владельцем почтового ящика может быть пользователь или ресурс, например Конференц-зал. Например, пользователю секретарю могут быть предоставлены права представителя для папки календаря конференц-зала, чтобы обрабатывать запросы на бронирование. Вы можете использовать управляемый API EWS или EWS, чтобы разрешить владельцу почтового ящика или администратору добавить делегата, указать, к каким папкам может получить доступ представитель, а затем задать разрешения для этой папки. Делегатам можно предоставлять доступ к следующим папкам: 
  
- Календарь
    
- Задачи
    
- Inbox;
    
- Контакты
    
- Примечания
    
- Журнал
    
Когда пользователь получает доступ к одной или нескольким этим папкам, они могут создавать, получать, обновлять, удалять, копировать и искать элементы в этой папке и всех дочерних папках в зависимости от [разрешений](#bk_delegateperms) , заданных для папки. Способ выполнения приложением этих действий зависит от того, требуется ли [явный](#bk_explicit) или [неявный](#bk_implicit) доступ. 
  
## <a name="delegate-permissions"></a>Делегирование разрешений
<a name="bk_delegateperms"> </a>

Когда администратор или владелец почтового ящика добавляет делегата к почтовому ящику, он также может задать уровень разрешений для одной или нескольких папок. Если уровень разрешений не задан для папки, то по умолчанию в качестве значения разрешения задано значение None. Несколько пользователей могут иметь один и тот же уровень разрешений для папки, и пользователи могут иметь разные уровни разрешений для разных папок. Если вы используете управляемый API EWS, вы используете свойство [делегатеусер. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.permissions%28v=exchg.80%29.aspx) , которое содержит одно из значений перечисления [делегатефолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) для каждой папки, чтобы задать разрешения представителя для папок. Если вы используете EWS, используйте элемент [делегатепермиссионс](https://msdn.microsoft.com/library/292badc7-bab3-4368-9d7c-9a8b7edb279b%28Office.15%29.aspx) для установки разрешений делегата, а элемент [пермиссионлевел](https://msdn.microsoft.com/library/87978600-3523-451e-a725-ef092c543e2a%28Office.15%29.aspx) — для определения уровня разрешений. 
  
**Таблица 2. Уровни разрешений для представителей**

|**Уровень разрешений**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Это значение используется по умолчанию для всех папок.  <br/> |
|Автор  <br/> |Представитель может читать и создавать элементы, а также изменять и удалять созданные ими элементы. Например, представитель может создавать запросы задач и приглашения на собрания непосредственно в папке "Календарь" владельца почтового ящика или в папке "Календарь", а затем отправлять один из элементов от имени владельца почтового ящика.  <br/> |
|Корректор  <br/> |Представитель может делать все, что может делать автор, а также изменять и удалять элементы, созданные владельцем почтового ящика.  <br/> |
|Reviewer  <br/> |Представитель может читать элементы; Например, представитель с разрешением на просмотр может читать сообщения в папке "Входящие" другого пользователя.  <br/> |
|Пользовательские  <br/> |Владелец почтового ящика предоставил настраиваемый набор разрешений для делегата.  <br/> |
   
Свойство управляемого API [делгатеусер. виевприватеитемс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser.viewprivateitems%28v=exchg.80%29.aspx) EWS и элемент [виевприватеитемс](https://msdn.microsoft.com/library/80b949ac-440c-4a01-b428-ebafb5b1b802%28Office.15%29.aspx) EWS — это глобальный параметр, который влияет на все папки владельца почтового ящика, в том числе всю почту, контакты, календарь, задачи, заметки и папки дневника. Вы не можете разрешить доступ к частным элементам только в одной папке. 
  
## <a name="explicit-access"></a>Явный доступ
<a name="bk_explicit"> </a>

Проще говоря, явный доступ является вводным способом для делегатов для выполнения действий в папках и элементах владельца почтового ящика. Явный доступ предоставляется представителю, когда он включает известное имя папки для папки владельца почтового ящика, а также SMTP-адрес владельца почтового ящика в запросе к серверу. Доступ является явным, так как запрос делегата явно указывает, что контекст для метода или операции является почтовым ящиком владельца почтового ящика, а не почтового ящика представителя.
  
Явный доступ определяет контекст для всех методов или операций, выполняемых над папками или элементами, которые перемещаются вперед. Все идентификаторы элементов и папок возвращаются, если явно задан явный доступ, однозначно идентифицирующий себя для владельца почтового ящика (хотя и не для читаемого человека). Таким образом, приложению не нужно снова указать SMTP-адрес владельца почтового ящика и еще раз; контекст скрыт в идентификаторах. После определения элемента или папки делегат фактически использует [неявный доступ](#bk_implicit) для изменения элемента. На следующем рисунке показан процесс получения явного и неявного доступа. 
  
**Рис. 2. Запрос явного и неявного доступа к элементу или папке**

![Схема, на которой показано приложение, отправляющее запрос на явный доступ, ответ от сервера, запрос на неявный доступ и ответ от сервера.](media/Ex15_Delegate_ExplictImplicit.png)
  
Вы можете задать явный доступ во многих различных сценариях. По сути, каждый раз, когда вы отправляете идентификатор папки в методе или операции, вы можете задать явный доступ. Это может быть поиск папок, Поиск встреч, получение элементов, поиск бесед и т. д.
  
### <a name="explicit-access-and-the-ews-managed-api"></a>Явный доступ и управляемый API EWS
<a name="bk_explicitewsma"> </a>

Вы можете инициировать явный доступ представителя с помощью любого из указанных ниже перегруженных методов, которые принимают входной параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) для определения целевой папки: 
  
- [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)
    
- [ExchangeService. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- И многое другое!
    
В каждом из этих методов можно использовать параметр **FolderId** для определения целевой папки владельца почтового ящика, как показано ниже. 
  
```cs
new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com");
```

Например, чтобы выполнить присоединение к папке Calendar, **FolderId** в этом методе **BIND** указывает имя ИЗВЕСТНОЙ папки и SMTP-адрес владельца почтового ящика. 
  
```cs
CalendarFolder calendar = CalendarFolder.Bind(service, new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), new PropertySet());
```

Указав известное имя папки и SMTP-адрес, делегат может привязываться к папке календаря владельца почтового ящика, тем самым получая явный доступ к папке. Все последующие запросы на [неявный доступ](#bk_implicit) к элементам в папке полагаются на контекст, возвращенный в идентификаторах элементов и идентификаторах папок. По сути, идентификаторы содержат контекст для подразумеваемых вызовов доступа делегата. Чтобы получить идентификатор элемента, который соответствует определенным условиям, используйте следующую строку. 
  
```cs
FindItemsResults<Item> results = service.FindItems(new FolderId(WellKnownFolderName.Calendar, "primary@contoso.com"), filter, view);
```

В этом случае возвращается идентификатор элемента, а затем делегат может использовать неявный доступ для внесения изменений в элемент с помощью идентификатора элемента.
  
Необязательно инициировать явный доступ до тех пор, пока не запросите идентификатор элемента или идентификатор папки, к которым вы не получили доступ через существующий явный доступ. 
  
### <a name="explicit-access-and-ews"></a>Явный доступ и EWS
<a name="bk_explicitewsma"> </a>

Вы можете инициировать явный доступ с помощью операций "@ [Folder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)", " [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)" или " [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ". Эти операции предоставляют возможность использовать элемент [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) для определения целевой папки. Элемент **дистингуишедфолдерид** содержит один необязательный дочерний элемент, элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) . Элемент **Mailbox** при использовании в качестве дочернего элемента элемента **дистингуишедфолдерид** указывает почтовый ящик для делегата, к которому необходимо получить доступ. Если вызывающий пользователь имеет разрешение на доступ к папке владельца почтового ящика, ответ будет содержать коллекцию идентификаторов для элементов или папок этого почтового ящика. Идентификаторы элементов и папок, возвращаемые в ответе, могут использоваться для неявного доступа делегата. 
  
## <a name="implicit-access"></a>Неявный доступ
<a name="bk_implicit"> </a>

Неявный доступ используется после получения делегатом идентификатора элемента или папки в почтовом ящике владельца почтового ящика, а делегату требуется обновить, удалить или скопировать элемент. Когда делегат использует этот идентификатор элемента или папки в запросе, изменения вносятся в элемент в почтовом ящике владельца почтового ящика. Представителю не нужно включать SMTP-адрес владельца почтового ящика. 
  
Например, если делегат имеет идентификатор одной из папок владельца почтового ящика, делегат может выполнить операцию **FindItem** с этой папкой, используя идентификатор папки, без явного определения почтового ящика владельца почтового ящика. На этом шаге делегат может выполнять действия с папкой владельца почтового ящика с помощью идентификаторов, возвращаемых в ответах. 
  
### <a name="implicit-access-and-the-ews-managed-api"></a>Неявный доступ и управляемый API EWS

Если метод [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) получил идентификатор элемента, этот идентификатор элемента можно использовать в последующем вызове метода [Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для привязывания к элементу. Затем можно вызвать метод [Item. Update](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx), [Item. Delete](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)или [Item. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) — или любой вызов метода, для которого требуется идентификатор элемента, если это необходимо для завершения задачи. Пока представитель имеет соответствующие разрешения для папки, содержащей элемент (и, если применимо, папка, в которую перемещается элемент), делегат может вносить изменения в соответствии с их уровнями разрешений. 
  
### <a name="implicit-access-and-ews"></a>Неявный доступ и EWS

Если операция [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) получила идентификатор элемента, этот идентификатор элемента можно использовать в последующих операциях [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для привязывания к элементу. Затем можно вызвать операцию [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), [DeleteItem](../web-service-reference/deleteitem-operation.md)или [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) (или любую операцию, для которой требуется идентификатор элемента, если это необходимо для завершения задачи). Пока представитель имеет соответствующие разрешения для папки, содержащей элемент (и, если применимо, папка, в которую перемещается элемент), делегат может вносить изменения в соответствии с их уровнями разрешений. 
  
## <a name="in-this-section"></a>В этой статье
<a name="bk_implicit"> </a>

- [Добавление и удаление делегатов с помощью EWS в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
    
- [Доступ к календарю как представителю с помощью EWS в Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к контактам как представителю с помощью EWS в Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к электронной почте как представителю с помощью EWS в Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Задание разрешений для папки другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с делегированием, в EWS в Exchange](handling-delegation-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)

- [Предоставление другим пользователям возможности управлять почтой и календарем](https://office.microsoft.com/outlook-help/allow-someone-else-to-manage-your-mail-and-calendar-HA102749417.aspx)  

- [Add — MailboxPermission](https://technet.microsoft.com/library/bb124097%28v=exchg.150%29.aspx)
    