---
layout: default-layout
title: Release Note - Dynamsoft Camera Enhancer
description: This is the documentation - Release Note page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, Release Note
needAutoGenerateSidebar: true
needGenerateH3Content: false
noTitleIndex: true
breadcrumbText: Release Note
---

# Release Notes

## 4.0

> First released: 08-10-2023

### Highlights

* Synchronized the features of different platforms:
  * Added take photo feature to iOS edition to capture images with higher quality.
  * Added tip features to mobile editions to display tip messages.
  * Extended Notes attribute to the DrawingItem classes of mobile editions to store more information.
  * Synchronized the coordinate base of different platforms. Support coordinate base setting of the DrawingItems and tip messages.
* API break changes:
  * Refactored the camera-controlling APIs of the CameraEnhancer class.
  * Refactored the UI configuration APIs.
  * Other minor changes on the API names and behaviors.

| Versions | Available Editions |
| -------- | ------------------ |
| 4.0.1 | [Android]({{ site.android }}release-note/release-notes-4.x.html#401-10262023){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-4.x.html#401-10262023){:target="_blank"} |
| 4.0.0 | [Android]({{ site.android }}release-note/release-notes-4.x.html#400-08102023){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-4.x.html#400-08102023){:target="_blank"} / [JavaScript]({{ site.js-rn }}release-notes-4.x.html#400-08242023){:target="_blank"} |

## 3.0

> First released: 07-27-2022

### Highlights

* Added flexible shape drawing logic.

| Versions | Available Editions |
| -------- | ------------------ |
| 3.3.8 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#338-10122023){:target="_blank"} |
| 3.3.7 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#337-10112023){:target="_blank"} |
| 3.3.6 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#336-09132023){:target="_blank"} |
| 3.3.5 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#335-08022023){:target="_blank"} |
| 3.3.4 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#334-04172023){:target="_blank"} |
| 3.3.3 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#333-04112023){:target="_blank"} |
| 3.3.2 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#332-04042023){:target="_blank"} |
| 3.3.1 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#331-02202023){:target="_blank"} |
| 3.3.0 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#330-02092023){:target="_blank"} |
| 3.2.0 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#320-12132022){:target="_blank"} |
| 3.1.0 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#310-10202022){:target="_blank"} |
| 3.0.1 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#301-08042022){:target="_blank"} |
| 3.0.0 | [JavaScript]({{ site.js-rn }}release-notes-3.x.html#300-07272022){:target="_blank"} |

&nbsp;

## 2.3

> First released: 03-21-2022

### Highlights

{%- include release-notes/product-highlight-2.3.0.md -%}

| Versions | Available Editions |
| -------- | ------------------ |
| 2.3.20 | [iOS]({{ site.ios }}release-note/release-notes-2.x.html#2320-03272023){:target="_blank"} |
| 2.3.12 | [iOS]({{ site.ios }}release-note/release-notes-2.x.html#2312-03162023){:target="_blank"} |
| 2.3.11 | [Android]({{ site.android }}release-note/release-notes-2.x.html#2311-02142023){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#2311-01102023){:target="_blank"} |
| 2.3.10 | [Android]({{ site.android }}release-note/release-notes-2.x.html#2310-12132022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#2310-12132022){:target="_blank"} |
| 2.3.5 | [Android]({{ site.android }}release-note/release-notes-2.x.html#235-11042022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#235-11152022){:target="_blank"} |
| 2.3.4 | [Android]({{ site.android }}release-note/release-notes-2.x.html#234-09222022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#234-11042022){:target="_blank"} |
| 2.3.3 | [Android]({{ site.android }}release-note/release-notes-2.x.html#233-08182022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#233-09222022){:target="_blank"} |
| 2.3.2 | [JavaScript]({{ site.js-rn }}release-notes-2.x.html#232-03282022){:target="_blank"} / [Android]({{ site.android }}release-note/release-notes-2.x.html#232-08022022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#232-08022022){:target="_blank"} |
| 2.3.1 | [JavaScript]({{ site.js-rn }}release-notes-2.x.html#231-03212022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#231-07112022){:target="_blank"} |
| 2.3.0 | [Android]({{ site.android }}release-note/release-notes-2.x.html#230-06282022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#230-06282022){:target="_blank"} |

&nbsp;

## 2.1

> First released: 12-16-2021

### Highlights

* Added class scan region configuration APIs and `RegionDefinition` for users to set the region of interest. The frames will be cropped based on the scan region to accelerate further frame processing.
* Fast mode setting parameters are opened for users to set via `updateAdvancedSettings`. The fast mode will be more flexible.

| Versions | Available Editions |
| -------- | ------------------ |
| 2.1.4 | [Android]({{ site.android }}release-note/release-notes-2.x.html#214-05262022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#214-05262022){:target="_blank"} |
| 2.1.3 | [Android]({{ site.android }}release-note/release-notes-2.x.html#213-03022022){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#213-03022022){:target="_blank"} |
| 2.1.1 | [Android]({{ site.android }}release-note/release-notes-2.x.html#211-12282021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#211-12282021){:target="_blank"} |
| 2.1.0 | [Android]({{ site.android }}release-note/release-notes-2.x.html#210-12162021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#210-12162021){:target="_blank"} / [JavaScript]({{ site.js-rn }}release-notes-2.x.html#210-01202022){:target="_blank"} |

&nbsp; 

## 2.0

> First released: 10-19-2021

### Highlights

* Simplified the usage of camera-control APIs. The new APIs are easier to use and covers more scenarios.
* Simplified the usage of camera enhancer features. Users can enable all required features via the method `enableFeatures` by inputting the combined enumeration value.
* Extended the features of `DCECameraView`. Users can add and personalize the overlays and viewfinder on the camera UI.
* Extended the features of `DCEFrame`. `DCEFrame` will store more frame information to cover more scenarios. In addition, the method `toBitmap/toUIImage` is added to enable users to convert `DCEFrame` to a system built-in image object.

| Versions | Available Editions |
| -------- | ------------------ |
| 2.0.0 | [JavaScript]({{ site.js-rn }}release-notes-2.x.html#200-10202021){:target="_blank"} / [Android]({{ site.android }}release-note/release-notes-2.x.html#200-10192021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-2.x.html#200-10192021){:target="_blank"} |

&nbsp; 

<div class="fold-panel-prefix"></div>

## 1.x Versions <i class="fa fa-caret-down"></i>

<div class="fold-panel-start"></div>

&nbsp; 

### 1.0

> First released: 04-29-2021

#### Highlights

* Dynamsoft Camera Enhancer is released. The following features are available:
  + Video Buffer
  + Frame Filter
  + Fast Mode
  + Auto-Zoom
  + Enhanced-Focus

| Versions | Available Editions |
| -------- | ------------------ |
| 1.0.3 | [Android]({{ site.android }}release-note/release-notes-1.x.html#103-07202021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-1.x.html#103-07202021){:target="_blank"} |
| 1.0.1 | [Android]({{ site.android }}release-note/release-notes-1.x.html#101-06102021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-1.x.html#101-06102021){:target="_blank"} |
| 1.0.0 | [Android]({{ site.android }}release-note/release-notes-1.x.html#100-04292021){:target="_blank"} / [iOS]({{ site.ios }}release-note/release-notes-1.x.html#100-04292021){:target="_blank"} |

<div class="fold-panel-end"></div>
