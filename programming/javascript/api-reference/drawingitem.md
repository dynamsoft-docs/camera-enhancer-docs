---
layout: default-layout
title: Dynamsoft Camera Enhancer JavaScript API - DrawingItem
description: This page shows the DrawingItem definitions of Dynamsoft Camera Enhancer JavaScript SDK.
keywords: camera enhancer, drawingitem, javascript, js
needAutoGenerateSidebar: true
needGenerateH3Content: true
noTitleIndex: true
breadcrumbText: DrawingItem
---

# DrawingItem

A DrawingItem can be one of seven types.

```typescript
type DrawingItem = DT_Rect | DT_Arc | DT_Line | DT_Polygon | DT_Text | DT_Image | DT_Group;
```

| Type Name | Description |
|---|---|
| [DT_Rect](#dtrect) | Defines a DrawingItem the shape of a rectangle. |
| [DT_Arc](#dtarc)   | Defines a DrawingItem the shape of a arc. |
| [DT_Line](#dtline) | Defines a DrawingItem the shape of a line. |
| [DT_Polygon](#dtpolygon) | Defines a DrawingItem the shape of a polygon. |
| [DT_Text](#dttext) | Defines a DrawingItem that draws text. |
| [DT_Image](#dtimage) | Defines a DrawingItem that draws an image. |
| [DT_Group](#dtgroup) | Defines a DrawingItem which is a combination of more than one DrawingItem of the other six types.  |

## DT_Rect

Defines a DrawingItem the shape of a rectangle.

```typescript
class DT_Rect { 
  public constructor(x: number, y: number, width: number, height: number, styleId?: number) { }; 
  // The coordinates of the upper-left corner of the rectangle, in pixels.
  x: number; y: number;
  // The dimentions of the rectangle, in pixels.
  width: number; height: number;
  // The media type.
  mediaType: "rect"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

## DT_Arc

Defines a DrawingItem the shape of a arc.

```typescript
class DT_Arc { 
  constructor(x: number, y: number, radius: number, startAngle: number, endAngle: number, styleId?: number) { }; 
  // The coordinates of the the center of the circle, in pixels.
  x: number; y: number;
  // The radius of the circle, in pixels.
  radius: number; 
  // The starting angle, in radians (0 is at the 3 o'clock position of the arc's circle).
  startAngle: number; 
  // The ending angle, in radians.
  endAngle: number; 
  // The media type.
  mediaType: "arc"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

## DT_Line

Defines a DrawingItem the shape of a line.

```typescript
class DT_Line { 
  public constructor(startPoint: Point, endPoint: Point, styleId?: number) { } 
  // The coordinates of the staring point, in pixels.
  startPoint: Point; 
  // The coordinates of the end point, in pixels.
  endPoint: : Point; 
  // The media type.
  mediaType: "line"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

**See also**

* [Point](point.md)

## DT_Polygon

Defines a DrawingItem the shape of a polygon.

```typescript
class DT_Polygon { 
  public constructor(vertices: Array<Point>, styleId?: number) { } 
  // The coordinates of all the vertices, in pixels.
  vertices: Array<Point>; 
  // The media type.
  mediaType: "polygon"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

**See also**

* [Point](point.md)

## DT_Text

Defines a DrawingItem that draws text.

```typescript
class DT_Text { 
  public constructor(text: string, x: number, y: number, styleId?: number) { } 
  // The coordinates of the point at which to begin drawing the text, in pixels.
  x: number; y: number;
  // The text to be drawn.
  text: string; 
  // The media type.
  mediaType: "text"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

## DT_Image

Defines a DrawingItem that draws an image.

```typescript
class DT_Image { 
  //NOTE: If an DT_Image instance has been constructed with an image, it can be replaced later with either an HTMLImageElement or an HTMLCanvasElement. However, an HTMLVideoElement can only be used during the constructing. 
  public constructor(HTMLImageElement | HTMLCanvasElement | HTMLVideoElement, x: number, y: number, styleId?: number) { } 
  // The coordinates of the point at which to begin drawing the image, in pixels.
  x: number; y: number;
  image: HTMLImageElement | HTMLCanvasElement | HTMLVideoElement; 
  // The media type.
  mediaType: "image"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string; 
  // The style ID expected to use for drawing this item. If left blank, the SDK will decide which style to use.
  styleId?: number;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```

## DT_Group

Defines a DrawingItem which is a combination of more than one DrawingItem of the other six types.

```typescript
class DT_Group { 
  public constructor(childItems: Array<DrawingItem>) { }
  // An array of drawingItems that form this drawingItem group.
  childItems: Array<DT_Rect | DT_Line | DT_Arc | DT_Text | DT_Polygon>; 
  // The media type.
  mediaType: "group"; 
  // The style selector. If left blank, the SDK will assume it's "default". Available values are "default" and "selected".
  styleSelector?: string;
  // The ID of a drawingLayer where the DrawingItem is drawn. Only assigned after it's added to the drawingLayer.
  readonly drawingLayerId: number;
} 
```