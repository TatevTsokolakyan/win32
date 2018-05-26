---
title: TB\_SETBOUNDINGSIZE message
description: Sets the bounding size for a multi-column toolbar control.
ms.assetid: f406d9e3-1c40-4317-8cf1-51706f4c6adf
keywords:
- TB_SETBOUNDINGSIZE message Windows Controls
topic_type:
- apiref
api_name:
- TB_SETBOUNDINGSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# TB\_SETBOUNDINGSIZE message

\[Intended for internal use; not recommended for use in applications. This message may not be supported in future versions of Windows.\]

Sets the bounding size for a multi-column toolbar control.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Must be zero.

</dd> <dt>

*lParam* 
</dt> <dd>

Pointer to a [**SIZE**](https://msdn.microsoft.com/library/windows/desktop/dd145106) structure whose **cy** member contains the bounding height. The **cx** member (the width) is ignored.

</dd> </dl>

## Return value

The return value is not used.

## Security Considerations

Using this message might compromise the security of your program.

## Remarks

The bounding size controls how buttons are organized into columns. If the toolbar control does not have the [**TBSTYLE\_EX\_MULTICOLUMN**](toolbar-extended-styles.md#tbstyle-ex-multicolumn) style, this message has no effect.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




