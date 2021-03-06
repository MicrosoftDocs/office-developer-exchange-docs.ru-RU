---
title: комплетедате
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: Элемент Комплетедате представляет дату завершения элемента.
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461424"
---
# <a name="completedate"></a>комплетедате

Элемент **комплетедате** представляет дату завершения элемента. 
  
```xml
<CompleteDate/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[Флаг](flag.md) <br/> |Указывает флаг для элемента почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее дату и время, является обязательным при использовании этого элемента.
  
## <a name="remarks"></a>Примечания

Установка **комплетедате** имеет тот же последствия, что и установка [PercentComplete](percentcomplete.md) в 100 или [состояние](status.md) на " **завершено**". В запросе, который задает по крайней мере два из этих свойств, Последнее обработанное свойство будет определять значение, заданное для этих элементов. Например, если [PercentComplete](percentcomplete.md) равен 100, **Комплетедате** — 1 января 2007, а [состояние](status.md) — **NotStarted**, а свойства передаются в потоке в таком порядке, то результатом будет установка для задачи [состояния](status.md) **NotStarted**, [комплетедате](completedate.md) — **null**, а [PercentComplete](percentcomplete.md) — 0. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание задач](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Удаление задач](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

