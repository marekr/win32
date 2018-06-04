---
title: IVMDisplay Width property
description: The Width property contains the current width, in pixels, of the virtual machine's display.
ms.assetid: b9a694cb-035c-4574-a8c3-30073d57dc19
keywords:
- Width property Virtual Server
- Width property Virtual Server , IVMDisplay interface
- IVMDisplay interface Virtual Server , Width property
- Width property Virtual Server , VMDisplay interface
- VMDisplay interface Virtual Server , Width property
topic_type:
- apiref
api_name:
- IVMDisplay.Width
- IVMDisplay.get_Width
- VMDisplay.Width
api_location:
- VsComInterfaces.h
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IVMDisplay::Width property

The **Width** property contains the current width, in pixels, of the virtual machine's display.

This property is read-only.

## Syntax


```C++
HRESULT get_Width(
  [out] long *displayPixelWidth
);
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>VMDisplay.Width( _
  ByRef displayPixelWidth _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The width, in pixels, of the virtual machine's display.

This property value is read-only.

## Error codes



| Name                                                                                          | Meaning                                                                |
|-----------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>              | The operation was successful.<br/>                               |
| <dl> <dt>E\_POINTER</dt> </dl>         | The parameter is **NULL**.<br/>                                  |
| <dl> <dt>VM\_E\_VM\_UNKNOWN</dt> </dl> | The virtual machine is invalid or is not currently running.<br/> |
| <dl> <dt>VM\_E\_NO\_DISPLAY</dt> </dl> | Unable to locate a valid display for the virtual machine.<br/>   |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error occurred.<br/>                               |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMDisplay**](ivmdisplay.md)
</dt> </dl>

 

 




