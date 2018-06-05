---
Description: Returns a Boolean value that indicates whether the private key is exportable.
ms.assetid: 56e72747-126d-4bb4-ac10-ced0acef388b
title: PrivateKey.IsExportable method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# PrivateKey.IsExportable method

\[The **IsExportable** method is available for use in the operating systems specified in the Requirements section. Instead, use the [**X509Certificate2.PrivateKey Property**](https://www.bing.com/search?q=**X509Certificate2.PrivateKey Property**) in the [**System.Security.Cryptography.X509Certificates**](https://www.bing.com/search?q=**System.Security.Cryptography.X509Certificates**) namespace.\]

The **IsExportable** method returns a Boolean value that indicates whether the private key is exportable.

## Syntax


```VB
PrivateKey.IsExportable()
```



## Parameters

This method has no parameters.

## Return value

If true, the private key is marked exportable.

## Remarks

The return value of this method is dependent on the [*cryptographic service provider*](https://www.bing.com/search?q=*cryptographic service provider*) (CSP) used. This method will return a trustworthy value if a Microsoft CSP is used. If the CSP is not a Microsoft CSP, the return value cannot be trusted to be accurate.

## Requirements



|                            |                                                                                        |
|----------------------------|----------------------------------------------------------------------------------------|
| Redistributable<br/> | CAPICOM 2.0 or later on Windows Server 2003 and Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## See also

<dl> <dt>

[**PrivateKey**](privatekey.md)
</dt> </dl>

 

 



