---
title: Синхронизация почтового ящика и веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: decf1eee-9743-44f3-9333-b3a01af3683e
description: Узнайте, как работает синхронизация почтовых ящиков при использовании EWS для доступа к Exchange.
localization_priority: Priority
ms.openlocfilehash: 5dc700c7feb9fce6121a27ee73fc1a58e88e643a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456262"
---
# <a name="mailbox-synchronization-and-ews-in-exchange"></a>Синхронизация почтового ящика и веб-службах Exchange

Узнайте, как работает синхронизация почтовых ящиков при использовании EWS для доступа к Exchange.
  
В Exchange для получения содержимого почтовых ящиков и изменения содержимого почтовых ящиков в Exchange используются два типа синхронизации.
  
- Синхронизация папок
    
- Синхронизация элементов
    
В этой статье рассказывается о типах синхронизации, принципах синхронизации, шаблонах разработки синхронизации и рекомендациях по синхронизации.
  
## <a name="folder-and-item-synchronization"></a>Синхронизация папок и элементов
<a name="bk_typesofsyncs"> </a>

Синхронизация папок синхронизирует структуру папок или иерархию папок. Синхронизация элементов синхронизирует элементы в папке. При синхронизации элементов необходимо синхронизировать каждую папку в почтовом ящике независимо друг от друга. Вы можете использовать веб-интерфейс EWS или управляемый API EWS в приложении, чтобы реализовать синхронизацию папок и элементов.
  
**Таблица 1. Операции служб EWS и методы управляемого API EWS для синхронизации папок и элементов**

|**Операция служб EWS**|**Метод управляемого API EWS**|
|:-----|:-----|
|[SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Метод ExchangeService. SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Метод ExchangeService. SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
Область выполняемой синхронизации зависит от того, является ли она начальной или текущей синхронизацией следующим образом:
  
- Начальная синхронизация синхронизирует все папки или элементы на сервере с клиентом. После первоначальной синхронизации клиент сохраняет состояние синхронизации для будущих синхронизаций. Состояние синхронизации представляет все изменения на сервере, которые сервер передает клиенту.
    
- Текущие синхронизации синхронизируют все элементы или папки, которые были добавлены, удалены или изменены с момента предыдущей синхронизации. Сервер использует состояние синхронизации для вычисления изменений, которые необходимо сообщить клиенту, во время каждого из текущих циклов синхронизации.
    
Каждый метод или операция синхронизации возвращает список изменений, а не фактическую папку или сообщение, которое изменилось. Изменения элементов и папок выводятся с помощью следующих типов изменений:
  
- Create — указывает, что в клиенте необходимо создать новый элемент или папку.
    
- Обновление — указывает, что элемент или папка необходимо изменить на клиенте.
    
- Delete — указывает, что необходимо удалить элемент или папку на клиенте.
    
- Реадстатечанже for EWS или Реадфлагчанже для управляемого API EWS — указывает на то, что состояние чтения элемента изменилось либо с непрочтенного на чтение, либо как непрочтенное.
    
В Exchange Online, Exchange Online в составе Office 365 и версиях Exchange, начиная с Exchange 2010 с пакетом обновления 2 (SP2), элементы и папки возвращаются в порядке от новых к старым. В предыдущих версиях Exchange элементы и папки возвращаются от старых к новым.
  
## <a name="how-does-ews-synchronization-work"></a>Как работает синхронизация EWS?
<a name="bk_howdoesitwork"> </a>

Если вы используете синхронизацию почтового ящика в первый раз, используйте процесс, как показано на рисунке 1. Несмотря на то что вы можете использовать другие [шаблоны проекта синхронизации](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns), рекомендуется использовать этот подход для масштабируемых приложений.
  
**Рис. 1. Первоначальный шаблон проекта синхронизации**

![Иллюстрация, показывающая шаблон проектирования начальной синхронизации. Клиент вызывает методы SyncFolderHierarchy и Load или GetItem, чтобы получить папки, затем вызывает методы SyncFolderItems и LoadPropertiesForItems или GetItem, чтобы получить элементы каждой папки.](media/Exchange2013_SyncInitial.png)
  
Если вы используете для синхронизации почтового ящика имеющееся состояние синхронизации, рекомендуем реализовать шаблон оформления, как показано на рисунке 2. 
  
**Рис. 2. Непрерывный шаблон проекта синхронизации**

![Иллюстрация, показывающая шаблон проектирования текущей синхронизации. Клиент получает уведомление, а затем вызывает метод SyncFolderHierarchy или SyncFolderItems, получает свойства, после чего обновляет клиент или флаг чтения.](media/Exchange2013_Sync_Ongoing.png)
  
## <a name="synchronization-design-patterns"></a>Шаблоны проекта синхронизации
<a name="bk_syncpatterns"> </a>

Вы можете использовать один из двух шаблонов проекта для синхронизации в приложении, чтобы почтовые ящики не превышали даты: Синхронизация на основе уведомлений или способ синхронизации.
  
Синхронизация на основе уведомлений, как показано на [рисунке 2](mailbox-synchronization-and-ews-in-exchange.md#bk_howdoesitwork), использует уведомления для оповещения клиента о вызове методов [SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) или [SYNCFOLDERHIERARCHY](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) для управляемого API EWS, а также в операциях EWS [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) или [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) . Этот тип синхронизации, как правило, рекомендуется для масштабируемых приложений, но он может быть не лучшим решением для всех. Синхронизация на основе уведомлений имеет следующие преимущества: 
  
- Уведомления оптимизированы для сокращения числа вызовов базы данных сервера Exchange. Очереди событий и подписки управляются сервером почтовых ящиков (или сервером клиентского доступа в Exchange 2010 и Exchange 2007); Однако Управление событиями и подписками использует меньше ресурсов, чем альтернатива, что чаще выполняет синхронизацию с базой данных Exchange. Кроме того, в Exchange предусмотрены специальные [политики регулирования](ews-throttling-in-exchange.md) для уведомлений и подписок, позволяющие защитить ресурсы. 
    
Однако также существуют некоторые недостатки использования синхронизации на основе уведомлений.
  
- Уведомления являются шумом, так как большинство сценариев включает несколько уведомлений для одной цели пользователя. Особенно это относится к папке Calendar. Например, при получении одного приглашения на собрание создаются несколько уведомлений об элементах и папках, в том числе уведомление о создании элемента и другой для изменения элемента. Один из способов устранения этого недостатка состоит в том, чтобы создать задержку в несколько секунд в [ходе вызова метода](https://msdn.microsoft.com/library/exchange/aa580274%28v=exchg.150%29.aspx.aspx) [Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobject.load%28v=exchg.80%29.aspx), [лоадпропертиесфоритемс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx), [GetItem](https://msdn.microsoft.com/library/exchange/aa565934%28v=exchg.150%29.aspx.aspx)или GetItem. В случае приглашения на собрание, если вы сразу же вызываете операцию **GetItem** , может быть один вызов для создания элемента и другой для изменения элемента. Вместо этого, задерживая вызов, вы можете вызвать операцию **GetItem** один раз и получить изменения, охватывающие создание и изменение элемента одновременно. 
    
- Уведомления добавляются в очередь на сервере почтовых ящиков, а подписки сохраняются на сервере почтовых ящиков. Если сервер почтовых ящиков, управляющий подпиской, недоступен, вы потеряли все новые уведомления, синхронизация почтового ящика не будет выполнена, и вам потребуется повторно подписаться на уведомления.
    
- Необходимо спланировать стратегии преодоления последствий в случае отказа в уведомлениях. Таким образом, второй подход, шаблон конструктора только для синхронизации, является более устойчивым к минимуму, чем синхронизация на основе уведомлений, так как для этого требуется, чтобы клиент управлял состояние синхронизации, нет проблем с сходством с сервером почтовых ящиков, управляющим подпиской.
    
При реализации в качестве рекомендуемого шаблон проекта подписки на основе уведомлений использует: 
  
- Уведомления для определения *времени* изменения данных. 
    
- Управляемый API EWS **SyncFolderHierarchy** или **SyncFolderItems** , а также операции с **SyncFolderHierarchy** или **SyncFolderItems** , чтобы определить, *какие* изменения были внесены, оптимизируя число возвращаемых событий синхронизации. Был ли новый элемент создан, обновлен или удален? Это все, что вам нужно знать из этих методов, не полагать их на список свойств изменений. (Не вызывайте метод **GetItem** или **лоадпропертиесфоритемс** для всех возвращенных элементов или папок). 
    
- С помощью методов **Load** или **лоадпропертиесфоритемс** в управляемом API EWS, а также для **GetItem** определения *способа* изменения данных и получения свойств с сервера при необходимости можно организовать пакетные запросы в зависимости от объема возвращаемых данных. За ним следует сравнение свойств клиента и только что возвращенных с сервера, а в конечном итоге создание, удаление или изменение элемента или папки на клиенте. 
    
Подход, используемый только для синхронизации, полностью зависит от методов **SyncFolderItems** и **SyncFolderHierarchy** EWS, а также операций **SyncFolderHierarchy** или **SyncFolderItems** EWS, которые можно либо вызвать постоянно, либо как событие времени. Кроме того, существуют преимущества и недостатки этого параметра. Такой подход является более устойчивым, так как состояние синхронизации хранится в клиенте на уровне почтового ящика, а также на любом сервере почтовых ящиков, поддерживающем подписку на уведомления, не обязательно. Способ синхронизации может продолжать отработку отказа почтовых ящиков из-за независимости от сервера почтовых ящиков. Однако метод синхронизации увеличивает задержку для пользователя, так как элементы синхронизируются периодически или периодически, а не в режиме реального времени при получении элементов. Такой подход также является более дорогостоящим, так как вы выполняете вызовы к базе данных Exchange, когда это возможно, не было внесено никаких изменений. 
  
## <a name="synchronization-best-practices"></a>Рекомендации по синхронизации
<a name="bk_bestpractices"> </a>

Для приложений с высоким уровнем масштабируемости рекомендуется придерживаться следующих рекомендаций для синхронизации почтовых ящиков в приложении.
  
- При вызове метода **SyncFolderItems** или **SyncFolderHierarchy** для управляемого API EWS используется значение _идонли_ для параметра _Property_ , а при использовании операций EWS **SyncFolderHierarchy** или **SyncFolderItems** для [сокращения числа вызовов](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) к базе данных Exchange используется значение **идонли** . Чем больше свойств вы запрашиваете в наборе свойств вызова **SyncFolderItems** или **SyncFolderHierarchy** , создаются дополнительные внутренние вызовы. Создается новый вызов RPC для каждого запрошенного значения свойства, в то время как только один вызов RPC получает все **итемидс** для запроса, не зависимо от количества результатов для отчета. Поэтому запрос **идонли** вызывает один вызов базы данных, а запрос контейнера свойств для субъекта и отправителя приводит к трем вызовам базы данных: один для **субъекта**, один для **отправителя**, а другой для **ItemId**.
    
- Не вызывайте методы **загрузки** или **ЛОАДПРОПЕРТИЕСФОРИТЕМС** управляемого API EWS, а также операции GetItem или **GetFolder** **GetItem** для каждого элемента в отклике синхронизации. Вместо этого выполните синтаксический анализ результатов; Найдите изменения, не требующие извлечения всех свойств, например, изменения состояния чтения. Если ответ включает изменение состояния чтения, просто обновите флаг на клиенте и все готово. нет необходимости получать все свойства элемента. И убедитесь, что вы не намерены дублировать усилия, внеся изменения, полученные из одного и того же клиента. Например, если в ответе синхронизации есть удаление элемента, а на локальном клиенте нет необходимости удалять сообщение еще раз или получить все свойства этого элемента. 
    
- Избегайте регулирования, выполнив следующие действия:
    
  - При вызове метода **Лоадпропертиесфоритемс** управляемого API EWS или операции EWS для **получения элементов в** пакете не следует выполнять пакет слишком большого количества элементов в запросе; в противном случае может потребоваться [регулирование](ews-throttling-in-exchange.md). Рекомендуем включить 10 элементов в пакет.
    
  - Не создавайте слишком много запросов в течение короткого промежутка времени. Это также приведет к регулированию и увеличить время отклика, а не сократит его. 
    
  - Если вы обрабатываете элементы пакета, пакетно все элементы с одинаковыми значениями для атрибутов **ID** и **чанжекэй** элемента [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . 
    
  - Если вы перерегулируете, остановите отправку запросов. Повторная отправка запросов позволяет продлить усилия по восстановлению. Вместо этого дождитесь, пока не истечет срок действия, а затем повторите попытку отправки запросов на синхронизацию.
    
- В зависимости от типа получаемого [события уведомления](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_eventtypes) : 
    
  - Для **NewMail** или **измененных** событий вызовите метод **SyncFolderItems** УПРАВЛЯЕМого API EWS или **EWS,** так как уведомления не предоставляют **чанжекэй**, а уведомления не вызывают изменений состояния чтения.
    
  - Для **удаленных** событий, если подписка на уведомление была активна до выполнения предыдущей синхронизации, просто удалите событие локально. Необязательно вызывать метод **SyncFolderItems** управляемого API EWS или **SyncFolderItems** EWS сразу же после удаления. 
    
  - Если **измененное** событие вызвано изменением состояния чтения, не вызывайте метод **ЛОАДПРОПЕРТИЕСФОРИТЕМС** управляемого API EWS или операцию EWS **GetItem** , просто измените флаг элемента. 
    
- При синхронизации данных календаря выполните указанные ниже действия.
    
  - Используйте подход, похожий на синхронизацию на основе уведомлений. Так как **синкфолдеритем** не включает в себя какую-либо логику календарей, используйте метод [FINDAPPOINTMENTS](https://msdn.microsoft.com/library/dd633767%28v=exchg.80%29.aspx) управляемого API EWS или [операцию FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для с элементом [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) , чтобы просматривать встречи между двумя ДАТАМИ, а затем вызывать **метод** управляемого API EWS или **операцию GetItem** для получения свойств элемента календаря. 
    
  - Не запрашиваться с помощью метода **FindAppointments** управляемого API EWS или операции **FindItem** для EWS с помощью элемента **CalendarView** . 
    
- При синхронизации папок поиска:
    
  - Используйте подход, похожий на синхронизацию на основе уведомлений. 
    
  - Используйте уведомления, чтобы определить, когда изменяются данные.
    
  - Так как вы не можете использовать **синкфолдеритем** в папке поиска, используйте упорядоченный и постраничный метод [FINDITEMS](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) управляемого API EWS или операцию **FindItem** с набором элементов [фрактионалпажеитемвиев](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) и [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , чтобы определить, что изменилось. 
    
  - Для получения данных используйте метод **Лоадпропертиесфоритемс** управляемого API EWS **или операцию EWS** . 
    
## <a name="filtered-synchronization"></a>Синхронизация с фильтрацией
<a name="bk_filteredsync"> </a>

Метод **SyncFolderItems** управляемого API EWS и операция EWS **SyncFolderItems** позволяют игнорировать определенные элементы на основе их Итемидс с помощью параметра _ИГНОРЕИТЕМИДС_ в управляемом API EWS или элементе [Ignore](https://msdn.microsoft.com/library/7789eec5-ceec-43f2-84d5-d0d15b734076%28Office.15%29.aspx) в EWS. Это идеальный вариант, если, например, пользователи начинают отвечать всем сообщениям электронной почты, отправленным всем сотрудникам компании. 
  
Может возникнуть вопрос: можно ли фильтровать мои уведомления (и, следовательно, только синхронизацию запуска) при изменении определенных свойств? Несмотря на то, что подписки на уведомления основываются на типе изменений (создание, обновление, удаление), а не обновляемом свойстве, вы не можете отфильтровать уведомления таким образом. Вместо этого можно выполнить следующие действия:
  
- Используйте шаблон дизайна подписки на основе уведомлений.
    
- Повторно вызовите методы **SyncFolderItems** и **SyncFolderHierarchy** для управляемого API EWS, указав для параметра Set _Свойства_ значение _идонли_ , чтобы сделать состояние синхронизации актуальным. Или, если используется EWS, операции **SyncFolderHierarchy** и **SyncFolderItems** можно выполнить многократно, указав для **басешапе** значение **идонли**. 
    
- Отказаться от ответа (не анализировать его или выполнять какие-либо сравнения свойств).
    
- Используйте метод **FindItems** управляемого API EWS или операцию **FindItem** , а также сортировку и страницу для предварительного заполнения элементов в фильтрованной области, о которых вы волнуете. 
    
- Используйте состояние синхронизации для продолжения вызова метода **SyncFolderItems** управляемого API EWS или операции **SyncFolderItems** EWS, но Отслеживайте только изменения в наборе отфильтрованных элементов. Если создаются новые элементы, необходимо убедиться в том, что эти новые элементы находятся в отфильтрованной области. 
    
## <a name="in-this-section"></a>В этой статье
<a name="bk_filteredsync"> </a>

- [Синхронизация папок с помощью EWS в Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Синхронизация элементов с помощью EWS в Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Метод SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx)
    
- [Метод SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)
    
- [Операция SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)
    
- [Операция SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)
    

