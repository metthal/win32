---
Description: Sent once to the CPlApplet function of a Control Panel application before the DLL containing the Control Panel application is released.
ms.assetid: 1afcb0d3-41a7-4fd8-9561-d96e1e8f0ddb
title: CPL\_EXIT message
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CPL\_EXIT message

Sent once to the [**CPlApplet**](/windows/desktop/api/Cpl/nc-cpl-applet_proc) function of a Control Panel application before the DLL containing the Control Panel application is released.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>Must be zero.</dd> <dt>

*lParam* 
</dt> <dd>Must be zero.</dd> </dl>

## Return value

If the [**CPlApplet**](/windows/desktop/api/Cpl/nc-cpl-applet_proc) function processes this message successfully, it should return zero.

## Remarks

This message is sent after the last [**CPL\_STOP**](cpl-stop.md) message is sent.

In response to this message, a Control Panel application must free any memory that it has allocated and perform global-level cleanup.

## Requirements



|                                     |                                                                                  |
|-------------------------------------|----------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                      |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                             |
| Header<br/>                   | <dl> <dt>Cpl.h</dt> </dl> |



## See also

<dl> <dt>

[**FreeLibrary**](https://msdn.microsoft.com/windows/desktop/823d3147-4ba8-4fe5-ade4-e5604f47eb0a)
</dt> </dl>

 

 



