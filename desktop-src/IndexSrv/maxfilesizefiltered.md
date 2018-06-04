---
Description: MaxFilesizeFiltered
ms.assetid: 94a6ec0a-3b5d-4a95-823d-aca234f21593
title: MaxFilesizeFiltered
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MaxFilesizeFiltered

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The **MaxFilesizeFiltered** entry is the maximum size of a file that the default filter will process for contents.

### Summary



|          |                |
|----------|----------------|
| Type:    | **REG\_DWORD** |
| Units:   | Kilobytes      |
| Default: | 256            |



 

### Remarks

If the default filter is used for a file that is bigger than the value of the **MaxFilesizeFiltered** entry, only the file properties are filtered.

This limit does not apply for the filtering of registered file types.

## Related topics

<dl> <dt>

[Catalog, Property, and Scope Registry Entries](catalog--property--and-scope-registry-entries.md)
</dt> <dt>

[Main Registry Entries](main-registry-entries.md)
</dt> </dl>

 

 


