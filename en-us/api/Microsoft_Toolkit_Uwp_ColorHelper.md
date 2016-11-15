---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_ColorHelper.htm
title: Microsoft.Toolkit.Uwp.ColorHelper API 
description: API page for Microsoft.Toolkit.Uwp.ColorHelper
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# ColorHelper class

This class provides static helper methods for colors.

## Members

The **ColorHelper** class has the following types of members:

### Methods

#### ToColor(System.String colorString)

Returns a color based on XAML color string.

##### Parameters



| Name | Description | Type |


#### ToHex(Windows.UI.Color color)

Converts a Color value to a string representation of the value in hexadecimal.

##### Parameters



| Name | Description | Type |


#### ToInt(Windows.UI.Color color)

Returns the color value as a premultiplied Int32 - 4 byte ARGB structure.

##### Parameters



| Name | Description | Type |


#### ToHsl(Windows.UI.Color color)

Converts an RGBA Color the HSL representation.

##### Parameters



| Name | Description | Type |


#### ToHsv(Windows.UI.Color color)

Converts an RGBA Color the HSV representation.

##### Parameters



| Name | Description | Type |


#### FromHsl(System.Double hue,System.Double saturation,System.Double lightness,System.Double alpha)

Returns a Color struct based on HSL model.

##### Parameters



| Name | Description | Type |


#### FromHsv(System.Double hue,System.Double saturation,System.Double value,System.Double alpha)

Returns a Color struct based on HSV model.

##### Parameters



| Name | Description | Type |
