---
layout: default-layout
title: Dynamsoft Camera Enhancer - CameraDLSLicenseVerificationListener
description: This is the documentation - CameraDLSLicenseVerificationListener page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, CameraDLSLicenseVerificationListener
needAutoGenerateSidebar: true
noTitleIndex: true
needGenerateH3Content: true
breadcrumbText: CameraDLSLicenseVerificationListener
---

# DCELicenseVerificationListener

The interface to handle callback when license verification messages are returned.

```java
interface com.dynamsoft.dce.DCELicenseVerificationListener
```

| Method | Description |
| ------ | ----------- |
| `DCELicenseVerificationCallback` | The call back of the license server. |

## DCELicenseVerificationCallback

The call back of the license server. Add the code in the callback function to react when the license server connection is successful or failed.

```java
void DCELicenseVerificationCallback(boolean var1, Exception var2);
```

**Parameters**

`[in, out] isSuccess`: Whether the license verification was successful.  
`[in, out] error`: The error message from the license server.

**Code Snippet**

```java
cameraEnhancer.initLicense("Put your license here", new DCELicenseVerificationListener() {
    @Override
    public void DCELicenseVerificationCallback(boolean isSuccess, Exception e) {
        if (!isSuccess) {
            e.printStackTrace();
        }
    }
});
```