---
title: requestOpen element
author: windows-driver-content
description: The requestOpen element is used to open an event notification message on the client computer.
ms.assetid: c1797295-9aca-4986-bd9d-482bb7049942
keywords: ["requestOpen element Print Devices"]
topic_type:
- apiref
api_name:
- requestOpen
api_type:
- Schema
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# requestOpen element


The **requestOpen** element is used to open an event notification message on the client computer.

The **requestOpen** element is defined in the *asyncui* namespace at this URI: http://schemas.microsoft.com/2003/print/asyncui/v1/request. (This resource may not be available in some languages and countries.)

Usage
-----

``` syntax
<requestOpen>
  child elements
</requestOpen>
```

Attributes
----------

There are no attributes.

## Child elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>balloonUI</strong>](balloonui.md)</p></td>
<td><p></p>
<p>An optional element that is used to display a message balloon on the client computer.</p></td>
</tr>
<tr class="even">
<td><p>[<strong>customUI</strong>](customui.md)</p></td>
<td><p></p>
<p>An optional element that specifies a custom user interface to be displayed on a client computer.</p></td>
</tr>
<tr class="odd">
<td><p>[<strong>messageBoxUI</strong>](messageboxui.md)</p></td>
<td><p></p>
<p>An optional element that is used to display a message box on the client computer.</p></td>
</tr>
</tbody>
</table>

## Parent elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[<strong>asyncPrintUIRequest</strong>](asyncprintuirequest.md)</p></td>
<td><p></p>
<p>A required element that describes a request issued by the printer driver to create a message on a client computer.</p></td>
</tr>
</tbody>
</table>

Examples
--------

The following code example opens an event notification message.

```
<?xml version="1.0" ?>
   <asyncPrintUIRequest
    xmlns="http://schemas.microsoft.com/2003/print/asyncui/v1/request">
    <v1>
      <requestOpen>
        <balloonUI iconID="1" resourceDll="IHV.dll">
          <title stringID="1234" resourceDll="IHV.dll" />
          <body stringID="100" resourceDll="IHV.dll">
            <parameter stringID="5" />
            <parameter stringID="1002" resourceDll="IHV.dll" />
          </body>
        </balloonUI>
      </requestOpen>
    </v1>
  </asyncPrintUIRequest>
```

## <span id="see_also"></span>See also


[**asyncPrintUIRequest**](asyncprintuirequest.md)

[**balloonUI**](balloonui.md)

[**customUI**](customui.md)

[**messageBoxUI**](messageboxui.md)

[**requestClose**](requestclose.md)

 

 




