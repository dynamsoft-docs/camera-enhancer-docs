---
layout: default-layout
title: Introduction - Dynamsoft Camera Enhancer
description: This is the documentation - introduction page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, introduction
needAutoGenerateSidebar: true
needGenerateH3Content: true
noTitleIndex: true
breadcrumbText: Introduction
---

# Overview of Dynamsoft Camera Enhancer

Dynamsoft Camera Enhancer (DCE) is an SDK specially designed to enhance camera frame acquisition process. Its basic camera manipulation features can save developers hundreds of lines of code for integrating camera in their applications. However, what make it unique are its advanced features on frame processing which empower the applications to focus only on high-quality frames and achieve high efficiency and accuracy.

## Main features

### Enhance Video Input

#### Video Buffer

DCE internally maintains a video buffer, which allows the image processing products to assess the video frames instantly when processing the video streaming. It reduce the time consumption of frame acquisition and improves the stability of video multi-frame processing.

The video buffer feature of DCE is inherited from the ImageSourceAdapter (ISA) which is the standard input interface of Dynamsoft Capture Vision (DCV).

#### Frame Filtering

There are two kinds of filtering features for you to skip the blurry video frames:

- Sensor filter: Filter out all the video frames produced when the device is shaking.
- Frame sharpness filter: Filter out the blurry video frames with the frame quality evaluation algorithm (less than 10ms per image).

By enabling the frame filtering features, you can:

- Prevent the long-time-consumption on processing the blurry image.
- Improve the accuracy of barcode decoding and text line recognizing.
- Improve the quality of the normalize document image.

> Note:
> A valid license is required when using this feature.

#### Enhanced Focus

Generally, auto-focus is supported by the majority of mobile devices. The ability to use the system auto-focus is kept when working with DCE so that you don't need to worry about the focus issues. For the low-end devices without auto-focus ability, DCE provides several additional focus modes:

- Continous focus with a user-define interval.
- Focus when the video frame quality decreased.
- Tap to focus.

> Note:
> A valid license is required when using this feature.

#### Auto Zoom

If the barcode reader is enabled at the same time when DCE is working, we can use the intermediate result of the barcode reader to predetermine the area of interest. DCE will let the camera zoom in to approach the interest area on the occasion that the system did not receive the final result but the intermediate result is available. The zoom factor will be reset if the application decodes on the barcode successfully.

<div align="center">
   <p><img src="../assets/auto-zoom.gif" alt="auto-zoom" width="20%" /></p>
   <p>Figure 1 – Auto-zoom Feature</p>
</div>

> Note:
> A valid license is required when using this feature.

#### Smart Torch

The torch light is helpful to support the image processing when the environment light is dark. There are 3 way for DCE powered camera to access the torch light:

- Use torch control APIs to turn on/off the torch light.
- Add a torch button with `setTorchButton`. You can also configure the size, position, and image of the button.
- Enable the `smart-torch` feature so that the torch button appears only when the environment light is low.

> Note:
> A valid license is required when using `smart-torch` feature.

#### Regular Camera Control

Last but not least, we incorporated camera control APIs in the SDK. The benefits of these APIs are:

- Enable users to add camera functionality with a few lines of code
- Unified experience on iOS/Android

In summary,

| Feature List           | Pricing                                           |
|------------------------|---------------------------------------------------|
| Regular Camera Control | Free                                              |
| Video Buffer           | Free                                              |
| Auto Zoom              | Advanced feature that requires a license.         |
| Enhanced Focus         | Advanced feature that requires a license.         |
| Frame Cropping         | Advanced feature that requires a license.         |
| Frame Filtering        | Advanced feature that requires a license.         |
| Smart torch            | Advanced feature that requires a license.         |

With these features, users can easily integrate the camera and enable certain features when required so that the rest of the application logic can get high-quality images to process, which results in:

- Speed up on barcode or text reading.
- Less misreading rate.
- More convenient timing out system
- High standard camera control.

### Interactive UI View

Two view classes are available for different usage scenarios.

#### CameraView for Video streaming processing

- Display the real-time video streaming.
- Visualize the `CapturedResults` on the view with simple code.
- Useful components that can be easily added to the view.

#### ImageEditorView for single Image Processing

Start from v3.x, `ImageEditorView` is available for users to draw editable UI elements to auxiliary the recognition of the image.

- Display the image to process.
- Visualize the `CapturedResults` on the view with simple code.
- Manually edit the result location to further improve the recognition accuracy.

<div align="center">
   <p><img src="../assets/dce-ddn-view.gif" alt="EditorView" width="20%" /></p>
   <p>Figure 2 – Scan and Edit on the ImageEditorView</p>
</div>

## Usage Scenarios

### Enhanced Video Streaming Processing

DCE aims at improving the user experience on video streaming processing. The camera controlling APIs and the advanced camera features enable users to customize the video source. You can use the focus, zoom, and resolution control to directly improve the video sharpness so that the image processing accuracy will be insured. You can also implement the pre-processings like set a scan region or enable the frame filter so that the image processing libraries will focus on the more valuable image data.

The DCE views ameliorate the video streaming processing on another aspect. DCE views are able to receive and recognize the results output by Dynamsoft Capture Vision. With the view configuring APIs, you can easily visualize the captured results on the view like highlighting the decoded barcodes or the detected document pages. The views are designed to be interactive. You can use the preset events of DCE UI elements or add your customized events to further improve the experience of your video streaming processing.

### Long-distance decoding

With the help of DCE, users no longer need to manually approach the barcode area when decoding on the barcode that far from the camera. When a barcode area is found but failed to be decoded, DCE enables the camera to zoom in to the barcode area automatically. Once the barcode is decoded successfully, the zoom factor will be restored to the default value.

### Low-end devices

Bounded up with camera performance, it is always a huge challenge for camera-related applications to perform well on low-end devices. DCE is breaking through these hardware issues by enabling high-standard autofocus and frame filter functions. DCE focus APIs enable users to apply high-standard focus settings, which help the devices to capture higher standard images. In the meanwhile, the frame filter pattern of DCE enables the application to skip processing the low-quality frames.

## Programming language

Dynamsoft Camera Enhancer is now available for the following programming languages:

- [**JavaScript**]({{site.js}}) for Browsers (with limited features at present)
- [**Java**]({{site.android}}) for Android
- [**Objective-C** & **Swift**]({{site.ios}}) for iOS
