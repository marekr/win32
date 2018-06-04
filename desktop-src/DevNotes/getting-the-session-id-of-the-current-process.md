---
Description: The following example x86 assembly code gets the Terminal Services session ID associated with the current process.
ms.assetid: 9fcb35cb-6813-46a5-aa38-e102f1b6b7dc
title: Getting the Session ID of the Current Process
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Getting the Session ID of the Current Process

\[The memory addresses specified by this example code may change in future releases of Windows. To ensure that your application will continue to run correctly in the future, your application must call [**GetCurrentProcessId**](https://msdn.microsoft.com/windows/desktop/a442e147-0db0-4911-94de-91728a4b277a) and then [**ProcessIdToSessionId**](https://msdn.microsoft.com/windows/desktop/99a3f047-705c-40bc-8cc2-055257a4f2b3) instead of the following sample code.\]

The following example x86 assembly code gets the Terminal Services session ID associated with the current process.

``` syntax
mov     eax,fs:[00000018]
mov     eax,[eax+0x30]
mov     eax,[eax+0x1d4]
```

 

 


