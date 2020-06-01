---
title: Посталаддресс (Персонапосталаддресстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: Элемент Посталаддресс указывает почтовый адрес пользователя.
ms.openlocfilehash: 9e316e5e0135c2d18fab4067241988c65eceec66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465389"
---
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="c5a20-103">Посталаддресс (Персонапосталаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="c5a20-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="c5a20-104">Элемент **посталаддресс** указывает почтовый адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5a20-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
```XML
<PostalAddress>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</PostalAddress>
```

 <span data-ttu-id="c5a20-105">**персонапосталаддресстипе**</span><span class="sxs-lookup"><span data-stu-id="c5a20-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5a20-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5a20-106">Attributes and elements</span></span>

<span data-ttu-id="c5a20-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c5a20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5a20-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5a20-108">Attributes</span></span>

<span data-ttu-id="c5a20-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5a20-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5a20-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5a20-110">Child elements</span></span>

<span data-ttu-id="c5a20-111">[Улица](street.md)  |  [City (город](city.md)  |  ) [State (состояние](state-ex15websvcsotherref.md)  |  ) [Country (страна](country.md)  |  ) [PostalCode](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Тип (строка)](type-string.md)  |  [Широта](latitude.md)  |  [Долгота](longitude.md)  |  [Точность](accuracy.md)  |  [Высота](altitude.md)  |  [Алтитудеаккураци](altitudeaccuracy.md)  |  [Форматтедаддресс](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [Локатионсаурце](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="c5a20-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5a20-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5a20-112">Parent elements</span></span>

[<span data-ttu-id="c5a20-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="c5a20-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="c5a20-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="c5a20-114">Remarks</span></span>

<span data-ttu-id="c5a20-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c5a20-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c5a20-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5a20-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5a20-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5a20-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5a20-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5a20-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5a20-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5a20-119">Schema name</span></span>  <br/> |<span data-ttu-id="c5a20-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5a20-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5a20-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5a20-121">Validation file</span></span>  <br/> |<span data-ttu-id="c5a20-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5a20-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5a20-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5a20-123">Can be empty</span></span>  <br/> ||
   

