---
layout: default-layout
Title: ErrorCode - Dynamsoft Core Enumerations
Description: The enumeration ErrorCode of Dynamsoft Core describes all error codes.
Keywords: Error code
needGenerateH3Content: true
needAutoGenerateSidebar: true
noTitleIndex: true
breadcrumbText: ErrorCode
codeAutoHeight: true
---

# Enumeration ErrorCode

`ErrorCode` describes the error code that can be output by the library.

<div class="sample-code-prefix template2"></div>
   >- Android
   >- Objective-C
   >- Swift
   >
>
```java
@Retention(RetentionPolicy.CLASS)
public @interface EnumErrorCode
{
   public static final int DCE_OK = 0;
   public static final int DCE_UNKNOWN = -10000;
   public static final int DCE_LICENSE_INVALID = -10001;
   public static final int DCE_LICENSE_EXPIRED = -10002;
   public static final int DCE_CAMERA_MODULE_NOT_EXIST = -10003;
   public static final int DCE_FILE_NOT_FOUND = -10004;
   public static final int DCE_JSON_PARSE_FAILED = -10005;
   public static final int DCE_CAMERA_ID_NOT_EXIST = -10006;
   public static final int DCE_PARAMETER_VALUE_INVALID = -10038;
   public static final int DCE_LICENSEKEY_NOT_MATCHED = -10043;
   public static final int DCE_REQUESTED_FAILED = -10044;
   public static final int DCE_NO_SENSOR = -10045;
   public static final int DM_NO_LICENSE = -20000;
   public static final int DM_HANDSHAKE_CODE_INVALID = -20001;
   public static final int DM_LICENSE_BUFFER_FAILED = -20002;
   public static final int DM_LICENSE_SYNC_FAILED = -20003;
   public static final int DM_DEVICE_NOT_MATCH = -20004;
   public static final int DM_BIND_DEVICE_FAILED = -20005;
   public static final int DM_LICENSE_INTERFACE_CONFLICT = -20006;
   public static final int DM_LICENSE_CLIENT_DLL_MISSING = -20007;
   public static final int DM_INSTANCE_COUNT_OVER_LIMITED = -20008;
   public static final int DM_LICENSE_INIT_SEQUENCE_FAILED = -20009;
   public static final int DM_TRIAL_LICENSE = -20010;
   public static final int DM_FAILED_TO_REACH_DLS = -20200;
} ErrorCode;
```
>
```objc
typedef NS_ERROR_ENUM(DSErrorDomain, DSErrorCode) {
   EnumDCEErrorCode_OK = 0,
   EnumDCEErrorCode_UNKNOWN = -10000,
   EnumDCEErrorCode_LICENSE_INVALID = -10001,
   EnumDCEErrorCode_LICENSE_EXPIRED = -10002,
   EnumDCEErrorCode_CAMERA_MODULE_NOT_EXIST = -10003,
   EnumDCEErrorCode_FILE_NOT_FOUND = -10004,
   EnumDCEErrorCode_JSON_PARSE_FAILED = -10005,
   EnumDCEErrorCode_CAMERA_ID_NOT_EXIST = -10006,
   EnumDCEErrorCode_PARAMETER_VALUE_INVALID = -10038,
   EnumDCEErrorCode_LICENSEKEY_NOT_MATCHED = -10043,
   EnumDCEErrorCode_REQUESTED_FAILED = -10044,
   EnumDCEErrorCode_NO_SENSOR = -10045,
   EnumDCEErrorCode_NO_LICENSE = -20000,
   EnumDCEErrorCode_HANDSHAKE_CODE_INVALID = -20001,
   EnumDCEErrorCode_LICENSE_BUFFER_FAILED = -20002,
   EnumDCEErrorCode_LICENSE_SYNC_FAILED = -20003,
   EnumDCEErrorCode_DEVICE_NOT_MATCH = -20004,
   EnumDCEErrorCode_BIND_DEVICE_FAILED = -20005,
   EnumDCEErrorCode_LICENSE_INTERFACE_CONFLICT = -20006,
   EnumDCEErrorCode_LICENSE_CLIENT_DLL_MISSING = -20007,
   EnumDCEErrorCode_INSTANCE_COUNT_OVER_LIMITED = -20008,
   EnumDCEErrorCode_LICENSE_INIT_SEQUENCE_FAILED = -20009,
   EnumDCEErrorCode_TRIAL_LICENSE = -20010,
   EnumDCEErrorCode_FAILED_TO_REACH_DLS = -20200
};
```
>
```swift
public enum ErrorCode : Int
{
   OK = 0,
   UNKNOWN = -10000,
   LICENSE_INVALID = -10001,
   LICENSE_EXPIRED = -10002,
   CAMERA_MODULE_NOT_EXIST = -10003,
   FILE_NOT_FOUND = -10004,
   JSON_PARSE_FAILED = -10005,
   CAMERA_ID_NOT_EXIST = -10006,
   PARAMETER_VALUE_INVALID = -10038,
   LICENSEKEY_NOT_MATCHED = -10043,
   REQUESTED_FAILED = -10044,
   NO_SENSOR = -10045,
   NO_LICENSE = -20000,
   HANDSHAKE_CODE_INVALID = -20001,
   LICENSE_BUFFER_FAILED = -20002,
   LICENSE_SYNC_FAILED = -20003,
   DEVICE_NOT_MATCH = -20004,
   BIND_DEVICE_FAILED = -20005,
   LICENSE_INTERFACE_CONFLICT = -20006,
   LICENSE_CLIENT_DLL_MISSING = -20007,
   INSTANCE_COUNT_OVER_LIMITED = -20008,
   LICENSE_INIT_SEQUENCE_FAILED = -20009,
   TRIAL_LICENSE = -20010,
   FAILED_TO_REACH_DLS = -20200
}
```
