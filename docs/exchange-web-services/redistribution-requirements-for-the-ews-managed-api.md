---
title: Требования к перераспределению для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Узнайте, как можно перераспределить сборки управляемого API EWS с приложением.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463827"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Требования к перераспределению для управляемого API EWS

Узнайте, как можно перераспределить сборки управляемого API EWS с приложением.
  
При проектировании приложения управляемого API EWS вы также захотите решить, как будет выпустить его для пользователей. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Распространение приложения управляемого API EWS

Если ваше приложение не размещается на сервере Exchange Server, вам потребуется перераспределить сборки управляемого API EWS. Загрузка управляемого API EWS содержит две сборки, которые можно перераспределить: Microsoft. Exchange. WebServices. dll и Microsoft. Exchange. WebServices. auth. dll. Когда вы разрабатываете приложение для управляемого API EWS, учитывайте следующие сведения:
  
- Управляемый API EWS был разработан таким образом, чтобы его можно было скачать и распространить вместе с приложением, предназначенным для сервера Exchange Server. Кроме того, приложение может скачать управляемый API EWS.
    
- Вы можете использовать управляемый API EWS для обмена данными с сервером Exchange, на котором работает Exchange Online, Exchange Online в составе Office 365, или локальной версией Exchange, начиная с Exchange Server 2007.
    
- В версиях управляемого API EWS, начиная с версии 2,1, вы можете установить API в глобальном кэше сборок (GAC). MSI автоматически добавит библиотеку DLL в глобальный кэш сборок и будет доступна на уровне компьютера, а не на уровне пользователя.
    
Условия лицензии включены в загрузку управляемого API EWS. Ознакомьтесь с условиями предоставления достоверных сведений о том, что можно сделать с помощью управляемого API EWS.
  
## <a name="see-also"></a>См. также


- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    
- [Управляемый API EWS (Загрузка)](https://aka.ms/ews-managed-api-readme)
    

