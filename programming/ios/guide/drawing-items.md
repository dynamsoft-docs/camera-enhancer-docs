---
layout: default-layout
title: Dynamsoft Camera Enhancer - Guide on iOS
description: This is the documentation - Guide on iOS page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, Guide on iOS
needAutoGenerateSidebar: true
noTitleIndex: true
needGenerateH3Content: true
breadcrumbText: iOS Guide
---

# UI Configurations

`DrawingItems` are the UI elements that user can create, modify and interact on the UI view. All the `DrawingItems` are contained in `DCEDrawingLayers` and finally displayed on the `DCECameraView` or `DCEImageEditorView`.

<div align="center">
    <p><img src="assets/drawing-items.png" width="70%" alt="drawing-item"></p>
    <p>DrawingItems in DCECameraView and DCEImageEditorView</p>
</div>

## Basic Usages

&nbsp;

### Display Highlight Overlays

When `DynamsoftCameraEnhancer(DCE)` is used together with other Dynamsoft products like `DynamsoftBarcodeReader(DBR)` and `DynamsoftDocumentNormalizer(DDN)`, it can automatically draw highlight overlays (`QuadDrawingItem`) on the detected barcodes or documents. If you want to disable this feature, you can use the following code to stop drawing the highlights.

```swift
// Example: Remove all highlights on the barcodes
editorView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID).setVisible(false);
```

<div class="sample-code-prefix"></div>
>- Objective-C
>- Swift
>
>1. 
```objc
DCEDrawingLayer *dbrLayer = [imageEditorView getDrawingLayer:DCEDrawingLayer.DBR_LAYER_ID];
drawingLayer
```
2. 
```swift
let dbrLayer = imageEditorView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID)
dbrLayer.visible = false
```

&nbsp;

### Style Configuration

You can change the style of the `DrawingItems` specifying a `DrawingStyleId`. The `DrawingStyleId` can be a preset `DrawingStyle` or a user-defined `DrawingStyle`.

To change the style of `DrawingItems` with preset `DrawingStyles`:

```swift
// You can change the drawing style of all DrawingItems in the layer.
cameraView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID).setDrawingStyleId(DrawingStyleManager.DEFAULT_STYLE_ID_3);
// You can also change the drawing style of a part of the DrawingItems.
editorView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID).setDrawingStyleId(DrawingStyleManager.DEFAULT_STYLE_ID_3, EnumDrawingItemState.DIS_SELECTED, EnumDrawingItemMediaType.DIMT_QUADRILATERAL});
```

<div class="sample-code-prefix"></div>
>- Objective-C
>- Swift
>
>1. 
```objc
DCEDrawingLayer *dbrLayer = [imageEditorView getDrawingLayer:DCEDrawingLayer.DBR_LAYER_ID];
// You can change the drawing style of all DrawingItems in the layer.
[dbrLayer setDrawingStyleId:DrawingStyleManager.DEFAULT_STYLE_ID_3];
// You can also change the drawing style of a part of the DrawingItems.
[dbrLayer setDrawingStyleId:DrawingStyleManager.DEFAULT_STYLE_ID_3 state:EnumDrawingItemStateSelected mediaType:EnumDrawingItemMediaTypeRectangle];
```
2. 
```swift
let dbrLayer = imageEditorView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID)
// You can change the drawing style of all DrawingItems in the layer.
dbrLayer.setDrawingStyleId(DrawingStyleManager.DEFAULT_STYLE_ID_3)
// You can also change the drawing style of a part of the DrawingItems.
dbrLayer.setDrawingStyleId(DrawingStyleManager.DEFAULT_STYLE_ID_3, state:EnumDrawingItemStateSelected, mediaType:EnumDrawingItemMediaTypeRectangle)
```

List of all available preset styles:

```objc
// DrawingItems on DDN layer are using this style as default.
#define DEFAULT_STYLE_ID_1 = 1;
// DrawingItems on DBR layer are using this style as default.
#define DEFAULT_STYLE_ID_2 = 2;
// DrawingItems on DLR layer are using this style as default.
#define DEFAULT_STYLE_ID_3 = 3;
// DrawingItems on user defined layer are using this style as default.
#define DEFAULT_STYLE_ID_4 = 4;
// DrawingItems on DDN layer are using this style as default if they are selected.
#define SELECTED_STYLE_ID_1 = 5;
// DrawingItems on DBR layer are using this style as default if they are selected.
#define SELECTED_STYLE_ID_2 = 6;
// DrawingItems on DLR layer are using this style as default if they are selected.
#define SELECTED_STYLE_ID_3 = 7;
// DrawingItems on user defined layer are using this style as default if they are selected.
#define SELECTED_STYLE_ID_4 = 8;
```

<div align="center">
    <p><img src="assets/drawing-styles.png" width="50%" alt="drawing-item"></p>
    <p>Preset DrawingStyles</p>
</div>

If you want to set other styles to your UI elements, you can add your personal defined `DrawingStyles`.

```swift
// Create a new DrawingStyle via DrawingStyle manager and get the style ID of the new style.
int myStyleId = DrawingStyleManager.createDrawingStyle(0xff00ff00,2,0xff00ff00,0xff00ff00,12,"sans-serif");
// Assign the newly created style to the targeting DrawingItems.
cameraView.getDrawingLayer(DCEDrawingLayer.DBR_LAYER_ID).setDrawingStyleId(myStyleId);
```

<div class="sample-code-prefix"></div>
>- Objective-C
>- Swift
>
>1. 
```objc
UIColor *strokeColour = [UIColor colorWithRed:0.2 green:0.3 blue:0.4 alpha:0.5];
UIColor *fillColour = [UIColor colorWithRed:0.2 green:0.3 blue:0.4 alpha:0.5];
UIColor *textColour = [UIColor colorWithRed:0.2 green:0.3 blue:0.4 alpha:0.5];
UIFont *textFont = [UIFont systemFontOfSize:12.0];
NSInteger myStyle = [DrawingStyleManager createDrawingStyle:strokeColour strokeWidth:2.0 fillColor:fillColour textColor:textColour font:textFont];
```
2. 
```swift
let strokeColor = UIColor.init(red: 0.2, green: 0.3, blue: 0.4, alpha: 0.5)
let fillColour = UIColor.init(red: 0.2, green: 0.3, blue: 0.4, alpha: 0.5)
let textColor = UIColor.init(red: 0.2, green: 0.3, blue: 0.4, alpha: 0.5)
let textFont = UIFont.systemFont(ofSize: 12, weight: UIFont.weight.light)
let myStyleID = DrawingStyleManager.createDrawingStyle(strokeColor, strokeWidth:1, fillColor:fillColor, textColor:textColor, font: textFont)
```

To modify the existing DrawingStyles:

```swift
// Get the style by ID.

// Modify the style.

```

<div class="sample-code-prefix"></div>
>- Objective-C
>- Swift
>
>1. 
```objc

```
2. 
```swift

```

&nbsp;

## Advanced Usages

&nbsp;

### Add User Defined UI Elements

Apart from the system-defined items, you can add your personal defined UI elements via the `DrawingItem` APIs. On this page, we will draw a user-defined `quadrilateral` on the `DCEImageEditorView` for example.

1. Create a new `QuadDrawingItem`.

   ```swift
   // Create a new quadrilateral.
   com.dynamsoft.core.Quadrilateral newQuad = new Quadrilateral();
   // Add your code to assign the quad data.
   newQuad.points = new com.dynamsoft.core.Point[]{new Point(0,0),new Point(100,0), new Point(100,100), new Point(0,100)};
   // Use the newly created quadrilateral to initialize the DrawingItem.
   DrawingItem item = new QuadDrawingItem(newQuad);
   ```

   <div class="sample-code-prefix"></div>
   >- Objective-C
   >- Swift
   >
   >1. 
   ```objc
   ```
   2. 
   ```swift
   ```

2. Add the Created `DrawingItems` to the view.

   ```swift
   // To display the drawingItems on the UI, you have to put the DrawingItems in a ArrayList.
   ArrayList<DrawingItem> drawingItems = new ArrayList<>();
   drawingItems.add(item);
   // The following code shows how to add the ArrayList of DrawingItems to the first layer of the cameraView.
   // There are multiple layers in DCECameraView and DCEImageEditorView.
   // You must select a layer for your DrawingItems.
   cameraView.getDrawingLayer(DCEDrawingLayer.DDN_LAYER_ID).addDrawingItems(drawingItems);
   // To add the DrawingItems to the imageEditorView
   // imageEditorView.getDrawingLayer(DCEDrawingLayer.DDN_LAYER_ID).addDrawingItems(drawingItems);
   ```

   <div class="sample-code-prefix"></div>
   >- Objective-C
   >- Swift
   >
   >1. 
   ```objc
   ```
   2. 
   ```swift
   ```

&nbsp;
