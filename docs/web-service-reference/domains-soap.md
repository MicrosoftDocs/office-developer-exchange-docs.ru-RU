---
title: Домены (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Элемент Domains представляет коллекцию доменов, которая возвращается в операции Жетдомаинсеттингс (SOAP), домены, для которых в организации используется операция Жетфедератионинформатион (SOAP), или домены с отношением Организации, возвращенные операцией Жеторганизатионрелатионшипсеттингс (SOAP).
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526307"
---
# <a name="domains-soap"></a>Домены (SOAP)

Элемент **Domains** представляет коллекцию доменов, которая возвращается в [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), домены, для которых в организации используется [Операция жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md), или домены с отношением Организации, возвращенные [операцией жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md).
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **Домены**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домен (SOAP)](domain-soap.md) <br/> |Представляет один домен.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетдомаинсеттингсрекуест (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[Отклик (Жетфедератионинформатион) (SOAP)](response-getfederationinformationsoap.md) <br/> |Содержит данные ответа [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Жеторганизатионрелатионшипсеттингсрекуест (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |Представляет запрос [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Жетдомаинсеттингсрекуест (SOAP)](getdomainsettingsrequest-soap.md)  
- [Жетфедератионинформатионреспонсе (SOAP)](getfederationinformationresponse-soap.md)

