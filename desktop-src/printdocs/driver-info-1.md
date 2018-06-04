---
Description: The DRIVER\_INFO\_1 structure identifies a printer driver.
ms.assetid: 9435192b-3eba-4937-8cd3-bff4e9eb84d3
title: DRIVER\_INFO\_1 structure
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: structure
ms.date: 05/31/2018
---

# DRIVER\_INFO\_1 structure

The **DRIVER\_INFO\_1** structure identifies a printer driver.

## Syntax


```C++
typedef struct _DRIVER_INFO_1 {
  LPTSTR pName;
} DRIVER_INFO_1, *PDRIVER_INFO_1;
```



## Members

<dl> <dt>

**pName**
</dt> <dd>

Pointer to a null-terminated string that specifies the name of a printer driver.

</dd> </dl>

## Requirements



|                                     |                                                                                                           |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                                |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                      |
| Header<br/>                   | <dl> <dt>Winspool.h (include Windows.h)</dt> </dl> |
| Unicode and ANSI names<br/>   | **\_DRIVER\_INFO\_1W** (Unicode) and **\_DRIVER\_INFO\_1A** (ANSI)<br/>                             |



## See also

<dl> <dt>

[Printing](printdocs-printing.md)
</dt> <dt>

[Print Spooler API Structures](printing-and-print-spooler-structures.md)
</dt> <dt>

[**EnumPrinterDrivers**](enumprinterdrivers.md)
</dt> </dl>

 

 



