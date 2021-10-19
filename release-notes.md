---
layout: default-layout
title: Dynamsoft Camera Enhancer - Release Note
description: This is the documentation - Release Note page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, Release Note
needAutoGenerateSidebar: true
needGenerateH3Content: false
noTitleIndex: true
breadcrumbText: Release Note
---

# Release Notes

## 2.0.0 (10/19/2021)

### Highlights

- Simplified the usage of camera-control APIs. The new APIs are easier to use and covers more scenarios.
- Simplified the usage of camera enhancer features. Users can enable all required features via the method `enableFeatures` by inputting the combined enumeration value.
- Extended the features of `DCECameraView`. Users can add and personalize the overlays and viewfinder on the camera UI.
- Extended the features of `DCEFrame`. `DCEFrame` will store more frame information to cover more scenarios. In addition, the method `toBitmap` is added to enable users to convert `DCEFrame` to a visible image.
- The camera UI will display a fuzzified image instead of the previously captured image when the camera UI is quit and resumed.

### Editions

| -- | -- | -- |
| [JavaScript]({{ site.js-rn }}) | [Android]({{ site.android-release-note }}) | [iOS]({{ site.ios-release-note }}) |