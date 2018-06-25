---
title: Функция CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760927"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="5a421-103">Функция CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="5a421-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="5a421-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5a421-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="5a421-105">Возвращает номер страницы в логической базы данных, соответствующий индекса указанного байта в файле физической базы данных.</span><span class="sxs-lookup"><span data-stu-id="5a421-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="5a421-106">Если смещение файла является недопустимым или функция **ErrCheckDbHeaders** не был вызван для баз данных, эта функция возвращает нуль (0).</span><span class="sxs-lookup"><span data-stu-id="5a421-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="5a421-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="5a421-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="5a421-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="5a421-108">ibFileOffset</span></span>
  
<span data-ttu-id="5a421-109">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="5a421-109">Input parameter.</span></span> <span data-ttu-id="5a421-110">Смещение в файле базы данных, в байтах.</span><span class="sxs-lookup"><span data-stu-id="5a421-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="5a421-111">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="5a421-111">Return value</span></span>

<span data-ttu-id="5a421-112">Номер логической страницы файла базы данных, которая включает в себя указанное смещение.</span><span class="sxs-lookup"><span data-stu-id="5a421-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a421-113">Замечания</span><span class="sxs-lookup"><span data-stu-id="5a421-113">Remarks</span></span>

<span data-ttu-id="5a421-114">Если параметр **ibFileOffset** является недопустимым, функция **PgnoFromFileOffset** возвращает нуль (0).</span><span class="sxs-lookup"><span data-stu-id="5a421-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="5a421-115">Если еще не вызов функции **ErrCheckDbHeaders** в экземпляре **CCheckSGFiles** **PgnoFromFileOffset** также возвращает нуль (0).</span><span class="sxs-lookup"><span data-stu-id="5a421-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="5a421-116">Необходимо вызвать **ErrCheckDbHeaders** для инициализации размер страницы базы данных и число страниц, выделенных заголовков базы данных.</span><span class="sxs-lookup"><span data-stu-id="5a421-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="5a421-117">**PgnoFromFileOffset** следует использовать для заполнения **Страница\_INFO** структура элементов при подготовке вызов **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="5a421-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="5a421-118">Параметр **rgPageInfo** для **ErrCheckDbPages** требуется каждого элемента в массиве структуру **PAGE_INFO** значениями членов **ulPgno** правильно инициализировать.</span><span class="sxs-lookup"><span data-stu-id="5a421-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="5a421-119">Если вы используете многопоточного приложения CHKSGFILES, можно вызвать функцию **PgnoFromFileOffset** в многопоточные части приложения.</span><span class="sxs-lookup"><span data-stu-id="5a421-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="5a421-120">Обратите внимание на то, что обычно вызов этой функции несколько раз для каждой базы данных проверки.</span><span class="sxs-lookup"><span data-stu-id="5a421-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="5a421-121">Требования</span><span class="sxs-lookup"><span data-stu-id="5a421-121">Requirements</span></span>

<span data-ttu-id="5a421-122">Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5a421-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="5a421-123">Учетная запись, приложения в разделе должен иметь разрешение на чтение базы данных и журналов файлов, которые должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="5a421-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

