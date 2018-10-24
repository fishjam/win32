---
Description: The wave/in device class consists of audio devices for low-level wave audio input.
ms.assetid: b2f32019-088f-4805-af7e-559a8179b1e6
title: wave/in
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# wave/in

The wave/in device class consists of audio devices for low-level wave audio input. You access these devices by using the wave functions, which are described in the Platform Software Development Kit (SDK). Devices in this class are associated with line devices that support the LINEMEDIAMODE\_AUTOMATEDVOICE media type, which is specified in the **dwMediaModes** member of the [**LINEDEVCAPS**](/windows/desktop/api/Tapi/ns-tapi-linedevcaps_tag) structure for the line device.

The [**lineGetID**](/windows/desktop/api/Tapi/nf-tapi-linegetid) and [**phoneGetID**](/windows/desktop/api/Tapi/nf-tapi-phonegetid) functions fill a [**VARSTRING**](/windows/desktop/api/Tapi/ns-tapi-varstring_tag) structure, setting the **dwStringFormat** member to the STRINGFORMAT\_BINARY value and appending this additional member:

``` syntax
DWORD DeviceId;  // identifier of audio device
```

The **DeviceId** member is the identifier of a closed audio device. You use this identifier in a call to the [**waveInOpen**](https://msdn.microsoft.com/en-us/library/Dd743847(v=VS.85).aspx) function to open the device for input. You can use the resulting device handle to record digitized audio data from the line or phone device.

Although a "wave" device class also exists for low-level wave audio devices, you should always use the wave/in device class for low-level wave input.

For more information about the wave functions, see [**Multimedia Functions**](https://msdn.microsoft.com/en-us/library/Dd743586(v=VS.85).aspx).

 

 


