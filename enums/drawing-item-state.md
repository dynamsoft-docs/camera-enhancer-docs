---
layout: default-layout
title: DrawingItemState - Dynamsoft Camera Enhancer Enumerations
description: The enumeration DrawingItemState of Dynamsoft Camera Enhancer describes the state of DrawingItems.
keywords:  DrawingItem, state
needGenerateH3Content: true
needAutoGenerateSidebar: true
noTitleIndex: true
breadcrumbText: DrawingItemState
---

# DrawingItemState

Enumeration `DrawingItemState` describes the state of DrawingItems.

<div class="sample-code-prefix template2"></div>
   >- JavaScript
   >- Android
   >- Objective-C
   >- Swift
   >
>
```javascript
export enum EnumDrawingItemState {
   // The state of the DrawingItem is the default state.
   DIS_DEFAULT = 1,
   // The state of the DrawingItem is selected.
   DIS_SELECTED = 2
}
```
>
```java
@IntDef({DIS_DEFAULT,DIS_SELECTED})
@Retention(RetentionPolicy.CLASS)
public @interface EnumDrawingItemState {
   // The state of the DrawingItem is the default state.
   public static final int DIS_DEFAULT = 1;
   // The state of the DrawingItem is selected.
   public static final int DIS_SELECTED = 2;
}
```
>
```objc
typedef NS_ENUM(NSInteger, DSDrawingItemState) {
   /**
    * The state of the DrawingItem is the default state.
    */
   DSDrawingItemStateDefault = 1,
   /**
    * The state of the DrawingItem is selected.
    */
   DSDrawingItemStateSelected = 2
};
```
>
```swift
public enum EnumDrawingItemState : Int{
   /**
    * The state of the DrawingItem is the default state.
    */
   default = 1
   /**
    * The state of the DrawingItem is selected.
    */
   selected = 2
}
```
