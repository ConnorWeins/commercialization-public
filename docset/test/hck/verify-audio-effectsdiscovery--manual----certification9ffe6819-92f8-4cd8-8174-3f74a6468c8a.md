---
author: joshbax-msft
title: Verify Audio EffectsDiscovery (Manual) - Certification
description: Verify Audio EffectsDiscovery (Manual) - Certification
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 9797cc0a-9fea-421b-bacd-51b2f049177d
---

# Verify Audio EffectsDiscovery (Manual) - Certification


-   Test1/Test2

    Use WinRT APIs to check for the existence of raw mode support on a capture or render audio device. To support raw mode, the driver must support the new DDI for audio signal processing modes.

-   Test3/Test4

    Check for effects that are turned on by default in capture or render device on raw or default streams. On raw streams, the only expected effects are endpoint mode effects such as speaker compensation or speaker protection. On render stream of the **Communication** category, no effects are expected other than endpoint effects. The presence of effects in the **Other** category can also fail the test.

-   Test 5/Test 6

    In this test, all effects are disabled and then raw and default streams are queried to ensure that no effects other than must-have effects are on in the pipeline. Must-have effects include endpoint effects that cannot or should not be turned off.

-   Manual tests:

    This test ensures that when each of the effects on the UI (Windows Store App UI, or Enhancements tab in Sound Control panel) is enabled, the effects list shows up correctly.

    The test will iterate through each render/capture device and show the initial list of default effects on raw and default streams. It then prompts you to enable the effects on the UI. You can enable the effects one at a time or all at once. You should pay attention to the list of effects displayed as they choose each option. This should be repeated for each device. After the tests are done, you should press **Enter** to proceed. You are asked if the list of effects displayed is accurate. You can select **Y** or **N** as answer.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>Device.Audio.Base.AudioProcessing</p>
<p>[See the device hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254483)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows RT 8.1 Windows 8.1 x64 Windows 8.1 x86 Windows Server 2012 R2</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~1 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Certification</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Manual</p></td>
</tr>
</tbody>
</table>

 

## Running the test


Before you run the test, complete the test setup as described in the test requirements: [Audio Device Testing Prerequisites](audio-device-testing-prerequisites.md).

## Troubleshooting


For troubleshooting information, see [Troubleshooting Audio Testing](troubleshooting-audio-testing.md).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20Verify%20Audio%20EffectsDiscovery%20%28Manual%29%20-%20Certification%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



