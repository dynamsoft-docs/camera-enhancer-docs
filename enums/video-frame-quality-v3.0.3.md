---
layout: default-layout
Title: FrameQuality - Dynamsoft Camera EnhancerEnumerations
Description: The enumeration FrameQuality of Dynamsoft Camera Enhancerdescribes the quality of video frames.
Keywords: Video frame quality
needGenerateH3Content: true
needAutoGenerateSidebar: true
noTitleIndex: true
breadcrumbText: FrameQuality
codeAutoHeight: true
---

# Enumeration FrameQuality

`FrameQuality` describes the quality of video frames.

<div class="sample-code-prefix template2"></div>
   >- JavaScript
   >- Android
   >- Objective-C
   >- Swift
   >- C++
   >
>
```javascript
enum EnumFrameQuality {
   /**The frame quality is measured to be high.*/
   VFQ_HIGH = 0,
   /**The frame quality is measured to be low.*/
   VFQ_LOW = 1,
   /**The frame quality is unknown.*/
   VFQ_UNKNOWN = 2
}
```
>
```java
public class EnumFrameQuality {
   /**The frame quality is measured to be high.*/
   public static final int VFQ_HIGH = 0;
   /**The frame quality is measured to be low.*/
   public static final int VFQ_LOW = 1;
   /**The frame quality is unknown.*/
   public static final int VFQ_UNKNOWN = 2;
}
```
>
```objc
typedef NS_ENUM(NSInteger, DSFrameQuality)
{
   /**The frame quality is measured to be high.*/
   FrameQualityHigh,
   /**The frame quality is measured to be low.*/
   FrameQualityLow,
   /**The frame quality is unknown.*/
   FrameQualityUnknown
};
```
>
```swift
public enum FrameQuality : Int
{
   /**The frame quality is measured to be high.*/
   high,
   /**The frame quality is measured to be low.*/
   low,
   /**The frame quality is unknown.*/
   unknown
}
```
>
```cpp
typedef enum FrameQuality {
   /**The frame quality is measured to be high.*/
   VFQ_HIGH,
   /**The frame quality is measured to be low.*/
   VFQ_LOW,
   /**The frame quality is unknown.*/
   VFQ_UNKNOWN
} FrameQuality;
```
