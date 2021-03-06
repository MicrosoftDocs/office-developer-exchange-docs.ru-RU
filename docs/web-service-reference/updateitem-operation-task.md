---
title: Операция UpdateItem (Task)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459807"
---
# <a name="updateitem-operation-task"></a>Операция UpdateItem (Task)

Операция UpdateItem используется для обновления свойств элемента задачи в хранилище Exchange.
  
## <a name="remarks"></a>Примечания

Вы не можете отправлять запросы задач с помощью веб-служб Exchange. Веб-службы Exchange могут возвращать запросы задачи, созданные в Майкрософтofficeoutlook. Если запрос задачи уже был отправлен, то запрос на обновление задачи возвратит ошибку.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Обновление текущего экземпляра повторяющейся задачи

Результат выполнения операции UpdateItem для повторяющихся задач отличается от результата операции UpdateItem для одной неповторяющейся задачи. Изменения, возникающие при возникновении повторяющейся задачи, приводят к созданию одноразовых задач при выполнении следующих обновлений:
  
1. Для свойства Status повторяющейся или повторяющейся задачи задано значение " **завершено**".
    
2. Изменена дата начала или Дата окончания повторяющейся задачи нонреженератинг.
    
Например, если запрос **UpdateItem** задает для выполнения повторяющейся задачи значение **true**, **упдатеитемреспонсе** будет включать новый идентификатор и чанжекэй, представляющие только что созданную одноразовую задачу. Идентификатор, который был включен в запрос, по-прежнему действителен, а повторяющаяся задача, представленная этим идентификатором, была обновлена для представления следующего вхождения. Чанжекэй, включенный в запрос, больше не является допустимым, так как повторяющаяся задача была обновлена. 
  
Вы можете использовать [операцию GetItem](getitem-operation.md) , чтобы получить последние **чанжекэй** для повторяющейся задачи. 
  
Для непериодических задач или последнего повторения повторяющейся задачи ответ UpdateItem возвращает тот же **идентификатор** , который был передан в него, и возвращает связанный обновленный **чанжекэй**.
  
## <a name="see-also"></a>См. также



[Операция UpdateItem](updateitem-operation.md)

