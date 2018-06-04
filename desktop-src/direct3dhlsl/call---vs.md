---
title: call - vs
description: Performs a function call to the instruction marked with the provided label.
ms.assetid: 3c1ec529-1ee4-40d9-8ce5-f8e7a61fde9c
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# call - vs

Performs a function call to the instruction marked with the provided label.

## Syntax



| call l\# |
|----------|



 

where l\# is a [label - vs](label---vs.md) marking the beginning of the subroutine to be called.

## Remarks



| Vertex shader versions | 1\_1 | 2\_0 | 2\_x | 2\_sw | 3\_0 | 3\_sw |
|------------------------|------|------|------|-------|------|-------|
| call                   |      | x    | x    | x     | x    | x     |



 

This instruction does the following:

1.  Push address of the next instruction to the return address stack.
2.  Continue execution from the instruction marked by the label.

In vertex shader 2\_0, nesting calls are not allowed.

In vertex shader 2\_x, the nesting depth is limited by the StaticFlowControlDepth element of the [**D3DVSHADERCAPS2\_0**](https://msdn.microsoft.com/library/windows/desktop/bb172635) structure. For more information, see [**GetDeviceCaps**](https://msdn.microsoft.com/library/windows/desktop/bb174320).

In vertex shader 3\_0, four levels of call nesting are allowed.

Only forward calls are allowed. This means that the location of the label inside the vertex shader should be after the call instruction referencing it.

If a call instruction is invoked inside [loop](loop---vs.md)...[endloop](endloop---vs.md) block, the value of the [Loop Counter Register](dx9-graphics-reference-asm-vs-registers-loop-counter.md) (aL) is accessible inside the subroutine.

If a subroutine is referencing the [Loop Counter Register](dx9-graphics-reference-asm-vs-registers-loop-counter.md) (aL) located outside of the subroutine, every instance of the call to this subroutine should be surrounded by a [loop](loop---vs.md)...[endloop](endloop---vs.md) block.

## Related topics

<dl> <dt>

[Vertex Shader Instructions](dx9-graphics-reference-asm-vs-instructions.md)
</dt> </dl>

 

 



