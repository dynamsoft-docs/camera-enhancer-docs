---
layout: default-layout
title: CoordinateBase - Dynamsoft Camera Enhancer Enumerations
description: The enumeration CoordinateBase of Dynamsoft Camera Enhancer describes the coordinate base.
keywords:  Coordinate base
needGenerateH3Content: true
needAutoGenerateSidebar: true
noTitleIndex: true
breadcrumbText: CoordinateBase
---

# CoordinateBase

Enumeration `CoordinateBase` describes the camera position.

<div class="sample-code-prefix template2"></div>
   >- Android
   >- Objective-C
   >- Swift
   >
>
```java
@IntDef({CB_IMAGE,CB_VIEW})
@Retention(RetentionPolicy.CLASS)
public @interface EnumCoordinateBase {
   // pixel, percentage
   public static final int CB_IMAGE = 0;
   // DP
   public static final int CB_VIEW = 1;
}
```
>
```objc
typedef NS_ENUM(NSInteger, DSCoordinateBase) {
   /**
    * Image coordinate.
    */
   DSCoordinateBaseImage = 0,
   /**
    * View coordinate.
    */
   DSCoordinateBaseView = 1
};
```
>
```swift
public enum CoordinateBase : Int{
   /**
    * Image coordinate.
    */
   image = 0
   /**
    * View coordinate.
    */
   view = 1
}
```
