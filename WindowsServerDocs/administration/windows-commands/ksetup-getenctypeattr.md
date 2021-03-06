---
title: ksetup:getenctypeattr
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 6c7ec002-355e-474d-bc27-27215049f1a8
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# ksetup:getenctypeattr



Retrieves the encryption type attribute for the domain.

## Syntax

```
ksetup /getenctypeattr <DomainName> 
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|\<DomainName>|Name of the domain to which you want to establish a connection. Use the fully qualified domain name or a simple form of the name, such as corp.contoso.com or contoso.|

## Remarks

To view the encryption type for the Kerberos ticket-granting ticket (TGT) and the session key, run the **klist** command and view the output.

If the command succeeds or fails, a status message is displayed upon successful or failed completion.

To set the domain that you want to connect to and use, run the **ksetup /domain \<DomainName>** command.

## Examples

Verify the encryption type attribute for the domain:
```
ksetup /getenctypeattr mit.contoso.com
```

## Additional References

-   [Klist](klist.md)
-   [Ksetup:domain](ksetup-domain.md)
-   [Ksetup:addenctypeattr](ksetup-addenctypeattr.md)
-   [Ksetup:setenctypeattr](ksetup-setenctypeattr.md)
-   [Ksetup:delenctypeattr](ksetup-delenctypeattr.md)
-   - [Command-Line Syntax Key](command-line-syntax-key.md)