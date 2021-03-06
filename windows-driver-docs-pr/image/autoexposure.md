---
title: AutoExposure element
description: The required AutoExposure element specifies that the WSD Scan Service should automatically determine the exposure settings for the document.
ms.assetid: ccc2b246-cfa1-4d79-b968-7b4bbaad17ee
keywords: ["AutoExposure element Imaging Devices"]
topic_type:
- apiref
api_name:
- wscn AutoExposure
api_type:
- Schema
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# AutoExposure element


The required **AutoExposure** element specifies that the WSD Scan Service should automatically determine the exposure settings for the document.

Usage
-----

``` syntax
<wscn:AutoExposure>
  text
</wscn:AutoExposure>
```

Attributes
----------

There are no attributes.

Text value
----------

Required. A Boolean value that must be 0, false, 1, or true.**falsetrue**

## Child elements


There are no child elements.

## Parent elements


<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>Exposure</strong>](exposure.md)</p></td>
</tr>
</tbody>
</table>

Remarks
-------

When the Boolean value of the **AutoExposure** element is 1 or **true**, the scan device will employ image processing techniques to reduce the background of the document to white.

When the value is 0 or **false**, the device should use the default settings for each of the exposure settings.

## <span id="see_also"></span>See also


[**Exposure**](exposure.md)

 

 






