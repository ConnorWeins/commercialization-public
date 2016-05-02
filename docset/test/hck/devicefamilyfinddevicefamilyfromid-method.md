---
author: joshbax-msft
title: DeviceFamily.FindDeviceFamilyFromId Method
description: DeviceFamily.FindDeviceFamilyFromId Method
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 6c85cc95-8b7b-4a4c-ab60-1a95c3864212
---

# DeviceFamily.FindDeviceFamilyFromId Method


This method retrieves a device family for the given hardware ID.

**Namespace:** Microsoft.Windows.Kits.Hardware.ObjectModel **Assembly:** Microsoft.Windows.Kits.Hardware.ObjectModel (in Microsoft.Windows.Kits.Hardware.ObjectModel)

## Usage


**Visual Basic**`Dim idToFind As String``Dim manager As ProjectManager``Dim returnValue As DeviceFamily``returnValue = DeviceFamily.FindDeviceFamilyFromId(idToFind, manager)`

## Syntax


**Visual Basic**`Public Shared Function FindDeviceFamilyFromId ( _`           `idToFind As String, _`           `manager As ProjectManager _``) As DeviceFamily`

**C#**`public static DeviceFamily FindDeviceFamilyFromId (`           `string idToFind,`           `ProjectManager manager``)`

## Parameters


*idToFind*      The hardware ID to use to compare against.

*manager*      The logoManager object against which to perform the search.

## Return Value


Returns **DeviceFamily**.

## Remarks


An exception occurs when the *idToFind* parameter or the *manager* parameter is **null** or the *idToFind* parameter is blank.

## Thread Safety


Any public static (**Shared** in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20DeviceFamily.FindDeviceFamilyFromId%20Method%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



