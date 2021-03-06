---
title: Функция функция cchksgfiles. Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447052"
---
# <a name="cchksgfilesdelete-function"></a>Функция функция cchksgfiles. Delete

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Уничтожает существующий экземпляр класса **функция cchksgfiles** . Эту функцию необходимо вызвать после завершения работы приложения с указанным объектом. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Параметры

### <a name="pcchecksgfiles"></a>пкчекксгфилес 
  
Входной параметр. Указатель на существующий объект **кчекксгфилес** . После этого память, связанная с объектом, будет освобождена. 
    
## <a name="return-value"></a>Возвращаемое значение

Нет.
  
## <a name="remarks"></a>Примечания

Функция **Delete** освобождает память, связанную с объектом **кчекксгфилес** . После вызова метода **Delete**указатель, переданный в параметре *пкчекксгфилес* , будет недопустимым, и для этого объекта невозможно выполнить другие операции. 
  
Если приложение использует функцию **еррчеккдбпажес** , приложение должно освободить буфер памяти вручную; Функция **удаления** не позволит освободить ее. 
  
Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **Delete** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** . 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.
  
Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.
  

