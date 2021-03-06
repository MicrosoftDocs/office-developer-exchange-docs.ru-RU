---
title: Address (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: Элемент Address представляет адрес электронной почты пользователя почтового ящика.
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463645"
---
# <a name="address-string"></a>Address (строка)

Элемент **Address** представляет адрес электронной почты пользователя почтового ящика. 
  
```xml
<Address>...</Address>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Электронная почта (EmailAddressType)](email-emailaddresstype.md) <br/> |Задает адрес электронной почты объекта MailboxData. Этот элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).<br/><br/> XPath для этого элемента:<br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (доступность)](mailbox-availability.md) <br/> | Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение.
  
## <a name="remarks"></a>Примечания

Этот элемент может встречаться не более одного раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) и элементе [Mailbox (Availability)](mailbox-availability.md) . 
  
> [!NOTE]
> Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserAvailability](getuseravailability-operation.md)
- [Операция GetUserOofSettings](getuseroofsettings-operation.md)
- [Операция SetUserOofSettings](setuseroofsettings-operation.md)
- [жетусераваилабилитирекуест](getuseravailabilityrequest.md)
- [жетусеруфсеттингсрекуест](getuseroofsettingsrequest.md)
- [сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md)
- [Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

