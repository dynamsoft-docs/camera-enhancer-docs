---
layout: default-layout
title: Enumerations Enhancer Features - Dynamsoft Camera Enhancer
description: This is the documentation - Enumerations Enhancer Features page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, Enumerations Enhancer Features
needAutoGenerateSidebar: true
breadcrumbText: Enumerations Enhancer Features
---

# EnumEnhancerFeatures

> You are viewing a history document page of Dynamsoft Camera Enhancer v2.x.

## Declarations

| Language | Declaration |
|----------|-------------|
| Java(Android) | `class EnumEnhancerFeatures` |
| Objective-C & Swift | `enum EnumEnhancerFeatures` |

## Members

| Member (Android) | Member (Objective-C) | Member (Swift) | Value | Description |
| ---------------- | -------------------- | -------------- | ----- | ----------- |
| `EF_FRAME_FILTER` | `EnumFRAME_FILTER` | `EnumFRAME_FILTER` | 0x01 | The frame sharpness filter feature of DCE. By enabling this feature, the low-quality frame will be recognized and discarded automatically. |
| `EF_SENSOR_CONTROL` | `EnumSENSOR_CONTROL` | `EnumSENSOR_CONTROL` | 0x02 | The sensor filter feature of DCE. By enabling this feature, the frames will be discarded automatically while the device is shaking. |
| `EF_ENHANCED_FOCUS` | `EnumENHANCED_FOCUS` | `EnumENHANCED_FOCUS` | 0x04 | The enhanced focus feature. DCE will support the camera in triggering auto-focus. |
| `EF_FAST_MODE` | `EnumFAST_MODE` | `EnumFAST_MODE` | 0x08 | The fast mode of DCE. By enabling the fast mode, the frames will be cropped to speed up the following processing. |
| `EF_AUTO_ZOOM` | `EnumAUTO_ZOOM` | `EnumAUTO_ZOOM` | 0x10 | The auto-zoom feature of DCE. By enabling this feature, the camera will automatically zoom in to the interest area. |
| `EF_SMART_TORCH` | `EnumSMART_TORCH` | `EnumSMART_TORCH` | 0x20 | Add a smart torch on the UI. The torch will be hided when the environment brightness is high and displayed when the brightness is low. |
| `EF_ALL` | `EnumALL` | `EnumALL` | 0x3f | Enable all the above features. |
