---
Description: Begins the process of canceling a pending asynchronous search.
title: IShellFolderSearchable::CancelAsyncSearch method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IShellFolderSearchable::CancelAsyncSearch method

Begins the process of canceling a pending asynchronous search.

## Syntax


```C++
HRESULT CancelAsyncSearch(
  [in] LPCITEMIDLIST pidlSearch,
  [in] DWORD         *pdwFlags
);
```



## Parameters

<dl> <dt>

*pidlSearch* \[in\]
</dt> <dd>

Type: **LPCITEMIDLIST**

A pointer to an [**ITEMIDLIST**](/windows/desktop/api/Shtypes/ns-shtypes-_itemidlist) for the search.

</dd> <dt>

*pdwFlags* \[in\]
</dt> <dd>

Type: **DWORD\***

No flags are currently defined; set to **NULL**.

</dd> </dl>

## Return value

Type: **HRESULT**

Returns S\_OK if canceling, or S\_FALSE if search is not running.

## Remarks

When the search is actually canceled, [**RunEnd**](ishellfoldersearchablecallback-runend.md) will be called.

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                             |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                   |
| DLL<br/>                      | <dl> <dt>Shell32.dll</dt> </dl> |



 

 



