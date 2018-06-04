---
Description: Determines the cross-product in four dimensions.
ms.assetid: 4f728fbd-cf5a-4d2e-ba4f-487616d83f6d
title: D3DXVec4Cross function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3DXVec4Cross function

Determines the cross-product in four dimensions.

## Syntax


```C++
D3DXVECTOR4* D3DXVec4Cross(
  _Inout_       D3DXVECTOR4 *pOut,
  _In_    const D3DXVECTOR4 *pV1,
  _In_    const D3DXVECTOR4 *pV2,
  _In_    const D3DXVECTOR4 *pV3
);
```



## Parameters

<dl> <dt>

*pOut* \[in, out\]
</dt> <dd>

Type: **[**D3DXVECTOR4**](https://msdn.microsoft.com/windows/desktop/fbfe7851-7bec-4fa0-b4dc-52f5cb83d0a4)\***

Pointer to the [**D3DXVECTOR4**](d3d10-d3dxvector4.md) that is the result of the operation.

</dd> <dt>

*pV1* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR4**](https://msdn.microsoft.com/windows/desktop/fbfe7851-7bec-4fa0-b4dc-52f5cb83d0a4)\***

Pointer to a source D3DXVECTOR4 structure.

</dd> <dt>

*pV2* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR4**](https://msdn.microsoft.com/windows/desktop/fbfe7851-7bec-4fa0-b4dc-52f5cb83d0a4)\***

Pointer to a source D3DXVECTOR4 structure.

</dd> <dt>

*pV3* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR4**](https://msdn.microsoft.com/windows/desktop/fbfe7851-7bec-4fa0-b4dc-52f5cb83d0a4)\***

Pointer to a source D3DXVECTOR4 structure.

</dd> </dl>

## Return value

Type: **[**D3DXVECTOR4**](https://msdn.microsoft.com/windows/desktop/fbfe7851-7bec-4fa0-b4dc-52f5cb83d0a4)\***

Pointer to a D3DXVECTOR4 structure that is the cross product.

## Remarks

The return value for this function is the same value returned in the pOut parameter. In this way, the D3DXVec4Cross function can be used as a parameter for another function.

## Requirements



|                   |                                                                                         |
|-------------------|-----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3DX10Math.h</dt> </dl> |



## See also

<dl> <dt>

[Math Functions](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 



