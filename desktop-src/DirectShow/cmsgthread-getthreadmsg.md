---
Description: Retrieves a queued CMsg object containing a request.
ms.assetid: 65b76121-c21c-4525-8dde-138783a4964e
title: CMsgThread.GetThreadMsg method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CMsgThread.GetThreadMsg method

Retrieves a queued [**CMsg**](cmsg.md) object containing a request.

## Syntax


```C++
virtual void GetThreadMsg(
   CMsg *msg
);
```



## Parameters

<dl> <dt>

*msg* 
</dt> <dd>

Pointer to an allocated [**CMsg**](cmsg.md) object.

</dd> </dl>

## Return value

This method does not return a value.

## Remarks

This member function is called from the worker thread's private [**ThreadProc**](camthread-threadproc.md) function to retrieve the next member function. The *msg* parameter should point to an allocated [**CMsg**](cmsg.md) object that will be filled with the parameters to the next request in the queue. If there are no queued requests, this member function blocks until the next request is queued (by a call to the [**CMsgThread::PutThreadMsg**](cmsgthread-putthreadmsg.md) member function).

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Msgthrd.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CMsgThread Class**](cmsgthread.md)
</dt> </dl>

 

 



