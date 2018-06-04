---
Description: Invokes the method that is called when the specified asynchronous action completes.
ms.assetid: 97199C1A-7CE3-4BBD-86A3-2CA9B27CC05E
title: AsyncActionCompletedHandler::Invoke method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# AsyncActionCompletedHandler::Invoke method

Invokes the method that is called when the specified asynchronous action completes.

## Syntax


```C++
HRESULT Invoke(
  [in] IAsyncAction *asyncInfo
);
```



## Parameters

<dl> <dt>

*asyncInfo* \[in\]
</dt> <dd>

Type: **[**IAsyncAction**](https://www.bing.com/search?q=**IAsyncAction**)\***

The asynchronous action that reports completion.

</dd> </dl>

## Return value

Type: **HRESULT**

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements



|                                     |                                                                                                   |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8<br/>                                                                              |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                                    |
| Header<br/>                   | <dl> <dt>Windows.Foundation.idl</dt> </dl> |



## See also

<dl> <dt>

[**AsyncActionCompletedHandler**](asyncactioncompletedhandler.md)
</dt> </dl>

 

 



