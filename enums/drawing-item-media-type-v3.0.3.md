---
layout: default-layout
title: DrawingItemMediaType - Dynamsoft Camera Enhancer Enumerations
description: The enumeration DrawingItemMediaType of Dynamsoft Camera Enhancer describes the media type of DrawingItems.
keywords:  DrawingItem, media type
needGenerateH3Content: true
needAutoGenerateSidebar: true
noTitleIndex: true
breadcrumbText: DrawingItemMediaType
permalink: /enums/drawing-item-media-type-v3.0.3.html
---

# DrawingItemMediaType

The enumeration `DrawingItemMediaType` describes the media type of DrawingItems.

<div class="sample-code-prefix template2"></div>
   >- Android
   >- Objective-C
   >- Swift
   >
>
```java
@Retention(RetentionPolicy.CLASS)
public @interface EnumDrawingItemMediaType {
   // The mediate type of the DrawingItem is rectangle.
   public static final int DIMT_RECTANGLE = 1;
   // The mediate type of the DrawingItem is quadrilateral.
   public static final int DIMT_QUADRILATERAL = 2;
   // The mediate type of the DrawingItem is text.
   public static final int DIMT_TEXT = 4;
   // The mediate type of the DrawingItem is line.
   public static final int DIMT_LINE = 8;
}
```
>
```objc
typedef NS_ENUM(NSInteger, DSDrawingItemMediaType) {
   /**
    * The mediate type of the DrawingItem is rectangle.
    */
   DSDrawingItemMediaTypeRectangle = 1,
   /**
    * The mediate type of the DrawingItem is quadrilateral.
    */
   DSDrawingItemMediaTypeQuadrilateral = 2,
   /**
    * The mediate type of the DrawingItem is text.
    */
   DSDrawingItemMediaTypeText = 4,
   /**
    * The mediate type of the DrawingItem is line.
    */
   DSDrawingItemMediaTypeLine = 8
};
```
>
```swift
public enum DrawingItemMediaType : Int{
   /**
    * The mediate type of the DrawingItem is rectangle.
    */
   rectangle = 1
   /**
    * The mediate type of the DrawingItem is quadrilateral.
    */
   quadrilateral = 2
   /**
    * The mediate type of the DrawingItem is text.
    */
   text = 4
   /**
    * The mediate type of the DrawingItem is line.
    */
   line = 8
}
```
