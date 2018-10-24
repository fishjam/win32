---
Description: A callback function used to notify the host when a texel value read has been completed.
MS-HAID: vspixengine.IPixEngine5Callbacks\_ReadTexelValueComplete\_UINT\_BSTR\_arr\_double\_arr
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: IPixEngine5Callbacks::ReadTexelValueComplete method
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# <span id="vspixengine.ipixengine5callbacks_readtexelvaluecomplete_uint_bstr_arr_double_arr"></span>IPixEngine5Callbacks::ReadTexelValueComplete method

A callback function used to notify the host when a texel value read has been completed.

## Syntax


```C++
);
```

## Parameters

*numChannels*   
The number of channels the texel has.

*count0\_channelNames*   
COM strings containing the names of the channels.

*count0\_channelValues*   
The values of the channels.

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

## <span id="see_also"></span>See also

[**IPixEngine5Callbacks**](https://msdn.microsoft.com/library/windows/desktop/mt432756)

 

 


