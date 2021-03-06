---
title: експанддлреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: Элемент Експанддлреспонсемессаже содержит состояние и результат одного запроса операции ExpandDL.
ms.openlocfilehash: e186c4e14cbb9c922a4d262c85c130b9c33ff939
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460640"
---
# <a name="expanddlresponsemessage"></a>експанддлреспонсемессаже

Элемент **експанддлреспонсемессаже** содержит состояние и результат одного запроса [операции ExpandDL](expanddl-operation.md) . 
  
- [експанддлреспонсе](expanddlresponse.md)  
- [респонсемессажес](responsemessages.md) 
- [експанддлреспонсемессаже](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

**експанддлреспонсемессажетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа [операции ExpandDL](expanddl-operation.md) .<br/><br/>Для этого атрибута допустимы следующие значения: <br/> <br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
|**индекседпагингоффсет** <br/> |Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения на страницы.  <br/> |
|**нумератороффсет** <br/> |Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробной части.  <br/> |
|**абсолутеденоминатор** <br/> |Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.  <br/> |
|**инклудесластитеминранже** <br/> |Указывает, что дополнительный разбиение по страницам не требуется. Этот атрибут будет иметь значение true, если текущие результаты содержат последний элемент в запросе.  <br/> |
|**тоталитемсинвиев** <br/> |Представляет общее число элементов, которые прошли ограничение.  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.<br/><br/> Ниже приведены примеры источников предупреждений.<br/>  <br/>— Хранилище Exchange находится в автономном режиме во время выполнения пакета.  <br/>-Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>— Почтовые ящики перемещаются.  <br/>— База данных почтовых ящиков (MDB) находится в автономном режиме.  <br/>— Срок действия пароля истек.  <br/>— Превышена квота.  <br/> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен.<br/><br/> Ниже приведены примеры источников ошибок.  <br/><br/>— Недопустимые атрибуты или элементы  <br/>— Атрибуты или элементы, которые выходят за пределы допустимого диапазона  <br/>— Неизвестный тег  <br/>— Атрибут или элемент, который не является допустимым в контексте  <br/>— Попытки несанкционированного доступа, выполняемые любым клиентом;  <br/>— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента <br/> <br/>  Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[мессажетекст](messagetext.md) <br/> |Предоставляет текстовое описание состояния отклика.  <br/> |
|[респонсекоде](responsecode.md) <br/> |Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.  <br/> |
|[дескриптивелинккэй](descriptivelinkkey.md) <br/> |В настоящее время не используется и зарезервировано для последующего использования. Он содержит значение 0.  <br/> |
|[мессажексмл](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке.  <br/> |
|[длекспансион](dlexpansion.md) <br/> |Содержит массив почтовых ящиков, содержащихся в списке рассылки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит ответные сообщения для запроса веб-служб Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExpandDL](expanddl-operation.md)
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

