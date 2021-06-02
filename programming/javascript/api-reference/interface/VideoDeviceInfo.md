---
layout: default-layout
title: Dynamsoft Barcode Reader JavaScript API Reference - BarcodeReader
description: This page shows the BarcodeReader Class of Dynamsoft Barcode Reader JavaScript SDK.
keywords: VideoDeviceInfo, BarcodeReader, api reference, javascript, js
needAutoGenerateSidebar: false
breadcrumbText: VideoDeviceInfo
---

Dynamsoft Barcode Reader SDK - JavaScript API
# VideoDeviceInfo

`interface` VideoDeviceInfo

* deviceId: *string*

* label: *string*

```js
let scanSettings = await scanner.getScanSettings();
scanSettings.intervalTime = 100; // 100ms
scanSettings.duplicateForgetTime = 3000; // 3s
await scanner.updateScanSettings(scanSettings);
```


