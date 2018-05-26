---
Description: Represents the association between Ethernet extensions and their capabilities.
ms.assetid: 6b32235a-175d-48f9-af3a-2d40f748a518
title: Msvm\_EthernetSwitchExtensionCapabilities class
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Msvm\_EthernetSwitchExtensionCapabilities class

Represents the association between Ethernet extensions and their capabilities.

The following syntax is simplified Managed Object Format (MOF) code, and it includes all of the inherited properties.

## Syntax

``` syntax
[Association, Aggregation, Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_EthernetSwitchExtensionCapabilities : CIM_ElementCapabilities
{
  Msvm_InstalledEthernetSwitchExtension  REF ManagedElement;
  Msvm_EthernetSwitchFeatureCapabilities REF Capabilities;
  uint16                                     Characteristics[];
};
```

## Members

The **Msvm\_EthernetSwitchExtensionCapabilities** class has these types of members:

-   [Properties](#properties)

### Properties

The **Msvm\_EthernetSwitchExtensionCapabilities** class has these properties.

<dl> <dt>

**Capabilities**
</dt> <dd> <dl> <dt>

Data type: **[**Msvm\_EthernetSwitchFeatureCapabilities**](msvm-ethernetswitchfeaturecapabilities.md)**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Capabilities")
</dt> </dl>

A reference to an instance of the [**Msvm\_EthernetSwitchFeatureCapabilities**](msvm-ethernetswitchfeaturecapabilities.md) class that represents the capabilities object associated with the switch. This property is inherited from [**CIM\_ElementCapabilities**](https://msdn.microsoft.com/library/mt446044).

</dd> <dt>

**Characteristics**
</dt> <dd> <dl> <dt>

Data type: **uint16** array
</dt> <dt>

Access type: Read-only
</dt> </dl>

Provides descriptive information about the capabilities. This property is inherited from [**CIM\_ElementCapabilities**](https://msdn.microsoft.com/library/mt446044).



| Value                                                                                                                                                                                                                       | Meaning                                                                                           |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| <span id="Default"></span><span id="default"></span><span id="DEFAULT"></span><dl> <dt>**Default**</dt> <dt>2</dt> </dl> | The associated capabilities represent the default capabilities of the managed element.<br/> |
| <span id="Current"></span><span id="current"></span><span id="CURRENT"></span><dl> <dt>**Current**</dt> <dt>3</dt> </dl> | The associated capabilities represent the current capabilities of the managed element.<br/> |



 

</dd> <dt>

**ManagedElement**
</dt> <dd> <dl> <dt>

Data type: **[**Msvm\_InstalledEthernetSwitchExtension**](msvm-installedethernetswitchextension.md)**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("ManagedElement")
</dt> </dl>

A reference to an instance of the [**Msvm\_InstalledEthernetSwitchExtension**](msvm-installedethernetswitchextension.md) class that represents the installed extension. This property is inherited from [**CIM\_ElementCapabilities**](https://msdn.microsoft.com/library/mt446044).

</dd> </dl>

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8 \[desktop apps only\]<br/>                                                              |
| Minimum supported server<br/> | Windows Server 2012 \[desktop apps only\]<br/>                                                    |
| Namespace<br/>                | Root\\Virtualization\\V2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



 

 



