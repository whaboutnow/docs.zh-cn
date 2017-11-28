---
title: "ICorProfilerInfo4 接口"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorProfilerInfo4
api_location: mscorwks.dll
api_type: COM
f1_keywords: ICorProfilerInfo4
helpviewer_keywords: ICorProfilerInfo4 interface [.NET Framework profiling]
ms.assetid: 80a5308e-c22f-4201-ba89-31cc8562515b
topic_type: apiref
caps.latest.revision: "9"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: db91347ad2c951c28ea7b653336450929d37bdcb
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2017
---
# <a name="icorprofilerinfo4-interface"></a><span data-ttu-id="38baf-102">ICorProfilerInfo4 接口</span><span class="sxs-lookup"><span data-stu-id="38baf-102">ICorProfilerInfo4 Interface</span></span>
<span data-ttu-id="38baf-103">提供代码探查器用于与公共语言运行时 (CLR)，从而控制事件监视并请求信息通信的方法。</span><span class="sxs-lookup"><span data-stu-id="38baf-103">Provides methods that code profilers use to communicate with the common language runtime (CLR) to control event monitoring and request information.</span></span> <span data-ttu-id="38baf-104">。</span><span class="sxs-lookup"><span data-stu-id="38baf-104">.</span></span> <span data-ttu-id="38baf-105">`ICorProfilerInfo4`接口是其他扩展`ICorProfilerInfo`接口。</span><span class="sxs-lookup"><span data-stu-id="38baf-105">The `ICorProfilerInfo4` interface is an extension of the other `ICorProfilerInfo` interfaces.</span></span> <span data-ttu-id="38baf-106">它提供了新方法，以支持实时 (JIT) 重新编译，在中添加[!INCLUDE[net_v45](../../../../includes/net-v45-md.md)]。</span><span class="sxs-lookup"><span data-stu-id="38baf-106">It provides new methods to support just-in-time (JIT) recompilation, added in the [!INCLUDE[net_v45](../../../../includes/net-v45-md.md)].</span></span>  
  
## <a name="methods"></a><span data-ttu-id="38baf-107">方法</span><span class="sxs-lookup"><span data-stu-id="38baf-107">Methods</span></span>  
  
|<span data-ttu-id="38baf-108">方法</span><span class="sxs-lookup"><span data-stu-id="38baf-108">Method</span></span>|<span data-ttu-id="38baf-109">描述</span><span class="sxs-lookup"><span data-stu-id="38baf-109">Description</span></span>|  
|------------|-----------------|  
|[<span data-ttu-id="38baf-110">EnumJITedFunctions2 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-110">EnumJITedFunctions2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-enumjitedfunctions2-method.md)|<span data-ttu-id="38baf-111">返回所有先前 JIT 编译和 JIT 重新编译的函数的枚举数。</span><span class="sxs-lookup"><span data-stu-id="38baf-111">Returns an enumerator for all functions that were previously JIT-compiled and JIT-recompiled.</span></span>|  
|[<span data-ttu-id="38baf-112">EnumThreads 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-112">EnumThreads Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-enumthreads-method.md)|<span data-ttu-id="38baf-113">获取一个枚举器，它提供方法以按顺序循环访问所分析进程中的所有托管线程的集合。</span><span class="sxs-lookup"><span data-stu-id="38baf-113">Gets an enumerator that that provides methods to sequentially iterate through the collection of all managed threads in the profiled process.</span></span>|  
|[<span data-ttu-id="38baf-114">GetCodeInfo3 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-114">GetCodeInfo3 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-getcodeinfo3-method.md)|<span data-ttu-id="38baf-115">获取本机代码的范围，该代码与指定函数的 JIT 重新编译版本相关联。</span><span class="sxs-lookup"><span data-stu-id="38baf-115">Gets the extents of native code associated with the JIT-recompiled version of the specified function.</span></span>|  
|[<span data-ttu-id="38baf-116">GetFunctionFromIP2 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-116">GetFunctionFromIP2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-getfunctionfromip2-method.md)|<span data-ttu-id="38baf-117">将托管的代码指令指针映射到指定的函数的 JIT 重新编译版本。</span><span class="sxs-lookup"><span data-stu-id="38baf-117">Maps a managed code instruction pointer to the JIT-recompiled version of a specified function.</span></span>|  
|[<span data-ttu-id="38baf-118">GetILToNativeMapping2 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-118">GetILToNativeMapping2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-getiltonativemapping2-method.md)|<span data-ttu-id="38baf-119">获取的 Microsoft 中间语言 (MSIL) 偏移量到本机偏移量指定的函数的 JIT 重新编译版本中包含的代码的映射。</span><span class="sxs-lookup"><span data-stu-id="38baf-119">Gets a map from Microsoft intermediate language (MSIL) offsets to native offsets for the code contained in the JIT-recompiled version of the specified function .</span></span>|  
|[<span data-ttu-id="38baf-120">GetObjectSize2 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-120">GetObjectSize2 Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-getobjectsize2-method.md)|<span data-ttu-id="38baf-121">返回指定对象的大小。</span><span class="sxs-lookup"><span data-stu-id="38baf-121">Returns the size of a specified object.</span></span>|  
|[<span data-ttu-id="38baf-122">GetReJITIDs 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-122">GetReJITIDs Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-getrejitids-method.md)|<span data-ttu-id="38baf-123">返回一个标识 JIT 重新编译的所有版本的指定的函数仍分配的 Id 数组。</span><span class="sxs-lookup"><span data-stu-id="38baf-123">Returns an array of IDs that identify all JIT-recompiled versions of the specified function that are still allocated.</span></span>|  
|[<span data-ttu-id="38baf-124">InitializeCurrentThread 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-124">InitializeCurrentThread Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-initializecurrentthread-method.md)|<span data-ttu-id="38baf-125">初始化之前在同一线程调用的 API，因此可以避免该死锁的后续探查器的当前线程。</span><span class="sxs-lookup"><span data-stu-id="38baf-125">Initializes the current thread in advance of subsequent profiler API calls on the same thread, so that deadlock can be avoided.</span></span>|  
|[<span data-ttu-id="38baf-126">RequestReJIT 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-126">RequestReJIT Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-requestrejit-method.md)|<span data-ttu-id="38baf-127">请求 JIT 重新编译指定函数的所有实例。</span><span class="sxs-lookup"><span data-stu-id="38baf-127">Requests a JIT recompilation of all instances of the specified functions.</span></span>|  
|[<span data-ttu-id="38baf-128">RequestRevert 方法</span><span class="sxs-lookup"><span data-stu-id="38baf-128">RequestRevert Method</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo4-requestrevert-method.md)|<span data-ttu-id="38baf-129">将指定函数的所有实例还原为其初始版本。</span><span class="sxs-lookup"><span data-stu-id="38baf-129">Reverts all instances of the specified functions to their original versions.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="38baf-130">备注</span><span class="sxs-lookup"><span data-stu-id="38baf-130">Remarks</span></span>  
 <span data-ttu-id="38baf-131">CLR 通过使用自由线程模型实现 `ICorProfilerInfo4` 接口的方法。</span><span class="sxs-lookup"><span data-stu-id="38baf-131">The CLR implements the methods of the `ICorProfilerInfo4` interface by using the free-threaded model.</span></span> <span data-ttu-id="38baf-132">每个方法均返回一个 HRESULT，指示成功或失败。</span><span class="sxs-lookup"><span data-stu-id="38baf-132">Each method returns an HRESULT to indicate success or failure.</span></span> <span data-ttu-id="38baf-133">有关可能的返回代码的列表，请参阅 CorError.h 文件。</span><span class="sxs-lookup"><span data-stu-id="38baf-133">For a list of possible return codes, see the CorError.h file.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="38baf-134">要求</span><span class="sxs-lookup"><span data-stu-id="38baf-134">Requirements</span></span>  
 <span data-ttu-id="38baf-135">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="38baf-135">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="38baf-136">**头文件：** CorProf.idl、CorProf.h</span><span class="sxs-lookup"><span data-stu-id="38baf-136">**Header:** CorProf.idl, CorProf.h</span></span>  
  
 <span data-ttu-id="38baf-137">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="38baf-137">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="38baf-138">**.NET framework 版本：**[!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="38baf-138">**.NET Framework Versions:** [!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="38baf-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="38baf-139">See Also</span></span>  
 [<span data-ttu-id="38baf-140">分析接口</span><span class="sxs-lookup"><span data-stu-id="38baf-140">Profiling Interfaces</span></span>](../../../../docs/framework/unmanaged-api/profiling/profiling-interfaces.md)  
 [<span data-ttu-id="38baf-141">ICorProfilerInfo 接口</span><span class="sxs-lookup"><span data-stu-id="38baf-141">ICorProfilerInfo Interface</span></span>](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo-interface.md)