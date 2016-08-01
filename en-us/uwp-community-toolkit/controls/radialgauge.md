---
permalink: /en-US/controls/radialgauge.html
title: RadialGauge XAML Control for UWP Community Toolkit
description: The RadialGauge Control displays a value in a certain range using a needle on a circular face
keywords: windows, app, toolkit, RadialGauge, gauge control, XAML, UWP, Radial, circular
layout: default
search.product: eADQiWindows 10XVcnh
---

# RadialGauge XAML Control
The **Radial Gauge Control** displays a value in a certain range using a needle on a circular face. This control will make data visualizations and dashboards more engaging with rich style and interactivity. 
The round gauges are powerful, easy to use, and highly configurable to present dashboards capable of displaying clocks, industrial panels, automotive dashboards, and even aircraft cockpits.

## How it works
The Radial Gauge supports animated transitions between configuration states. The control gradually animates as it redraws changes to the needle, needle position, scale range, color range, and more. 

## Syntax
```xaml
<controls:RadialGauge x:Name="RadialGaugeControl"
	Column="1"
	Value="70"
	Minimum="0"
	Maximum="180"
	TickSpacing="20"
	ScaleWidth="26"
	Unit="Units"
	TickBrush="Gainsboro"
	ScaleTickBrush="{ThemeResource ApplicationPageBackgroundThemeBrush}"
	UnitBrush="Black"
	ValueBrush="Black" 
	NeedleWidth="5" 
	TickLength="18">
</controls:RadialGauge>
```
## Example Image

## Example Code
<p> **Note:** Refer to the following project for example code that must be used when creating a using this toolkit for Universal Windows application development.<p>

[RadialGauge Sample Page](https://github.com/Microsoft/UWPCommunityToolkit/tree/master/Microsoft.Toolkit.Uwp.SampleApp/SamplePages/RadialGauge)

## Default Template 
[RadialGauge XAML File](https://github.com/Microsoft/UWPCommunityToolkit/blob/master/Microsoft.Toolkit.Uwp.UI.Controls/RadialGauge/RadialGauge.xaml) is the XAML template used in the toolkit for the default styling.

## Platforms 
Windows 10 SDK 10586 or higher

## API
Please view the [toolkit sample application](https://github.com/Microsoft/UWPCommunityToolkit/tree/master/Microsoft.Toolkit.Uwp.SampleApp) for the UWP Community Toolkit for samples of all the controls.

[RadialGauge API Docs](https://github.com/Microsoft/UWPCommunityToolkit-docs/blob/master/en-us/uwp-community-toolkit/api/Microsoft_Toolkit_Uwp_UI_Controls_RadialGauge.md)
