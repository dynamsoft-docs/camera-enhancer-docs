---
layout: home-page
title: Dynamsoft Camera Enhancer SDK – Documentation Overview
keywords: dynamsoft camera enhancer, dce, documentation, camera control, frame filtering
breadcrumbText: HomePage
description: Documentation home for Dynamsoft Camera Enhancer (DCE), the SDK that handles camera control and video frame acquisition for barcode, label and document scanning apps on Web, Android and iOS.
---

# Dynamsoft Camera Enhancer Documentation

`Dynamsoft Camera Enhancer (DCE)` is an SDK for camera control and video frame acquisition. It opens and configures the camera, keeps a video buffer that other Dynamsoft products read frames from, and filters out blurry or shaking frames so that recognition runs only on high-quality images. Its video buffer implements the Image Source Adapter (ISA), the standard input interface of [Dynamsoft Capture Vision](/capture-vision/docs/core/), so DCE can feed frames directly to Dynamsoft Barcode Reader, Label Recognizer, Document Normalizer and Code Parser.

## Platform Documentation

* Web (Client Side):
  * [JavaScript](/camera-enhancer/docs/web/){:target="_blank"}
* Mobile:
  * [Android API Reference](/camera-enhancer/docs/mobile/programming/android/api-reference.html){:target="_blank"}
  * [iOS API Reference](/camera-enhancer/docs/mobile/programming/ios/api-reference.html){:target="_blank"}

## Shared Concepts

These pages apply to every edition:

* [Introduction]({{ site.introduction }}) – main features: video buffer, frame filtering, enhanced focus, auto zoom and more.
* [Parameter Reference]({{ site.parameter-reference }}) – settings you can configure.
* [Enumerations]({{ site.enumerations }}) – camera state, camera position, resolution, frame quality and other enums.
* [License Activation]({{ site.license_activation }}License.html)
* [Trouble Shooting]({{ site.faq }})
