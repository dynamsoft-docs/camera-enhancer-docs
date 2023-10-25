---
layout: default-layout
title: License initialization - Dynamsoft Camera Enhancer
description: This is the documentation - License initialization page of Dynamsoft Camera Enhancer.
keywords:  Camera Enhancer, License initialization
needAutoGenerateSidebar: true
breadcrumbText: License Initialization
---

# License initialization

## Get a trial key

* A time-limited public trial key is available for every new device for the first use of Dynamsoft Camera Enhancer. The public trial key is the default key used in samples. You can also find the public trial key on the following parts of this page.
* If your free key is expired, please visit <a href="https://www.dynamsoft.com/customer/license/trialLicense?package=mobile&product=dce" target="_blank">Private Trial License Page</a> to get an extension.

## Get a full license

* [Contact us](https://www.dynamsoft.com/company/contact/)  to purchase a full license

## Initialize the license

The following code snippets are using the public trial key to initialize the license. You can replace the public trial key with your own license key.

1. Include `DynamsoftLicense` library.

2. Add the following code:

<div class="sample-code-prefix"></div>
>- Java(Android)
>- Objective-C
>- Swift
>
```java
LicenseManager.initLicense("DLS2eyJvcmdhbml6YXRpb25JRCI6IjIwMDAwMSJ9", this, (isSuccess, error) -> {
    if (!isSuccess) {
        error.printStackTrace();
    }
});
```
>
```objc
@interface AppDelegate () <DSLicenseVerificationListener>
@end
@implementation AppDelegate
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
    // Override point for customization after application launch.
    [DSLicenseManager initLicense:@"DLS2eyJvcmdhbml6YXRpb25JRCI6IjIwMDAwMSJ9" verificationDelegate:self];
    return YES;
}
- (void)onLicenseVerified:(BOOL)isSuccess error:(nullable NSError *)error {
    if (!isSuccess && error != nil) {
        NSLog(@"error: %@", error);
    }
}
```
>
```swift
@main
class AppDelegate: UIResponder, UIApplicationDelegate, LicenseVerificationListener {
    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
        // Override point for customization after application launch.
        LicenseManager.initLicense("DLS2eyJvcmdhbml6YXRpb25JRCI6IjIwMDAwMSJ9", verificationDelegate: self)
        return true
    }
    func onLicenseVerified(_ isSuccess: Bool, error: Error?) {
        if !isSuccess {
            if let error = error {
                print("\(error.localizedDescription)")
            }
        }
    }
}
```
