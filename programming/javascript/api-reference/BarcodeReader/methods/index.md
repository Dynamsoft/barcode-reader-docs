---
layout: default-layout
title: Dynamsoft Barcode Reader JavaScript API Reference - BarcodeReader Methods
description: This page shows BarcodeReader methods of Dynamsoft Barcode Reader JavaScript SDK.
keywords: methods, BarcodeReader, api reference, javascript, js
needAutoGenerateSidebar: false
breadcrumbText: Methods
---

# Dynamsoft Barcode Reader SDK - JavaScript BarcodeReader Class

The `BarcodeReader` class is used for **image** decoding.

## `BarcodeReader` *Class* Methods

### Initialize

The following methods are related to the initialization of `BarcodeReader` instances.

| Method               | Description |
|----------------------|-------------|
| [`createInstance`](initialize-and-destroy.md#createinstance) | Create a  `BarcodeReader` instance. |
| [`detectEnvironment`](initialize-and-destroy.md#detectenvironment) | Detect the current environment. |
| [`isLoaded`](initialize-and-destroy.md#isloaded) | Check if the decoding module is loaded. |
| [`loadWasm`](initialize-and-destroy.md#loadwasm) | Manually load and compile the decoding WASM module. |

## `BarcodeReader` *Instance* Methods

### Destroy

| Method               | Description |
|----------------------|-------------|
| [`destroy`](initialize-and-destroy.md#destroy) | Destroy the `BarcodeReader` instance. |

### Decode

The following methods are related to decoding barcodes.

| Method               | Description |
|----------------------|-------------|
| [`decode`](decode.md#decode) | Decode barcodes from images, binary data, URLs, and more. |
| [`decodeBase64String`](decode.md#decodebase64string) | Decode barcodes from a base64 encoded string. |
| [`decodeBuffer`](decode.md#decodebuffer) | Decode barcodes from raw buffer. |
| [`decodeUrl`](decode.md#decodeurl) | Decode barcodes from a URL. |

### Parameter and Runtime Settings

The following methods are related to customizing mode and runtime settings.

| Method               | Description |
|----------------------|-------------|
| [`getRuntimeSettings`](parameter-and-runtime-settings.md#getruntimesettings) | Get current runtime settings. |
| [`resetRuntimeSettings`](parameter-and-runtime-settings.md#resetruntimesettings) | Reset runtime settings to default. |
| [`updateRuntimeSettings`](parameter-and-runtime-settings.md#updateruntimesettings) | Modify and update the current runtime settings. |
| [`getModeArgument`](parameter-and-runtime-settings.md#getmodeargument) | Get argument value for the specified mode parameter. |
| [`setModeArgument`](parameter-and-runtime-settings.md#setmodeargument) | Set argument value for the specified mode parameter. |