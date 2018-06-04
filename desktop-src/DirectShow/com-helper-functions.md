---
Description: These functions provide support for implementing the IUnknown interface in DirectShow.
ms.assetid: 991e4c69-7d30-4ecf-9ccf-4920452c21d6
title: COM Helper Functions
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# COM Helper Functions

These functions provide support for implementing the **IUnknown** interface in DirectShow.



| Function                                               | Description                                                           |
|--------------------------------------------------------|-----------------------------------------------------------------------|
| [**DECLARE\_IUNKNOWN**](declare-iunknown.md)          | Declares the three methods of the base interface for a new interface. |
| [**GetInterface**](getinterface.md)                   | Retrieves an interface pointer to the requested client.               |
| [**INonDelegatingUnknown**](inondelegatingunknown.md) | Nondelegating version of the **IUnknown** interface.                  |
| [**LoadOLEAut32**](loadoleaut32.md)                   | Loads the Automation DLL (OleAut32.dll).                              |



 

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Combase.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[Utility Functions](utility-functions.md)
</dt> </dl>

 

 



