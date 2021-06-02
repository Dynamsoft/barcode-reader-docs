---
layout: default-layout
title: Dynamsoft Barcode Reader JavaScript API Reference - BarcodeReader
description: This page shows the BarcodeReader Class of Dynamsoft Barcode Reader JavaScript SDK.
keywords: RuntimeSettings, BarcodeReader, api reference, javascript, js
needAutoGenerateSidebar: false
breadcrumbText: RuntimeSettings
---

Dynamsoft Barcode Reader SDK - JavaScript API
# RuntimeSettings

`interface` RuntimeSettings

* barcodeFormatIds: *number | EnumBarcodeFormat*

  > Sets the formats of the barcode in BarcodeFormat group 1 to be read. Barcode formats in BarcodeFormat group 1 can be combined.
  > ```js
  > let runtimeSettings = await reader.getRuntimeSettings();
  > runtimeSettings.barcodeFormatIds = Dynamsoft.DBR.EnumBarcodeFormat.BF_ONED | Dynamsoft.DBR.EnumBarcodeFormat.BF_QR_CODE;
  > await reader.updateRuntimeSettings(runtimeSettings);
  > ```

  <br>

* barcodeFormatIds_2: *number | EnumBarcodeFormat_2*

  > Sets the formats of the barcode in BarcodeFormat group 2 to be read. Barcode formats in BarcodeFormat group 1 can be combined.

  <br>

* binarizationModes: *EnumBinarizationMode[]*

  <br>

* deblurLevel: *number*

  > Sets the degree of blurriness of the barcode.

  <br>

* expectedBarcodesCount: *number*

  > Sets the number of barcodes expected to be detected for each image.

  <br>

* furtherModes: *any*

  <br>

* intermediateResultTypes: *EnumIntermediateResultType*

  <br>

* localizationModes: *number[] | EnumLocalizationMode[]*

  > Sets the mode and priority for localization algorithms.

  <br>

* minBarcodeTextLength: *number*

  <br>

* minResultConfidence: *number*

  <br>

* PDFReadingMode: *EnumPDFReadingMode*

  > Not available in JS.

  <br>

* region: *RegionDefinition | RegionDefinition[]*

  > Sets the region definition including the regionTop, regionLeft, regionRight, regionBottom and regionMeasuredByPercentage.
  >
  > ```js
  > // Use a region of center 50% width and 50% height
  > let runtimeSettings = await reader.getRuntimeSettings();
  > runtimeSettings.region.regionLeft = 25;
  > runtimeSettings.region.regionTop = 25;
  > runtimeSettings.region.regionRight = 75;
  > runtimeSettings.region.regionBottom = 75;
  > runtimeSettings.region.regionMeasuredByPercentage = true;
  > await reader.updateRuntimeSettings(runtimeSettings);
  > ```
  >
  > Experimental feature:
  >
  > In [BarcodeScanner](../BarcodeScanner.md), `region` can be an array. For example `region = [r0, r1, r2]`, 0th frame use `r0`, 1st use `r1`, 2nd use `r2`, 3rd use `r0`, and then loop like this. 
  >
  > ```js
  > let runtimeSettings = await reader.getRuntimeSettings();
  > runtimeSettings.region = [
  >   null, // full image
  >   {regionLeft:25,regionTop:25,regionRight:75,regionBottom:75,regionMeasuredByPercentage:true}, // center 50% 
  >   {regionLeft:5,regionTop:45,regionRight:95,regionBottom:55,regionMeasuredByPercentage:true}, // width 90%, height 10% 
  > ];
  > await reader.updateRuntimeSettings(runtimeSettings);
  > ```

  <br>

* resultCoordinateType: *number | EnumResultCoordinateType*

  <br>

* returnBarcodeZoneClarity: *number*

  <br>

* scaleDownThreshold: *number*

  <br>

* scaleUpModes: *EnumScaleUpMode[]*

  <br>

* terminatePhase: *EnumTerminatePhase*

  <br>

* textResultOrderModes: *EnumTextResultOrderMode[]*

  <br>

* timeout: *number*

  > Sets the maximum amount of time (in milliseconds) that should be spent searching for a barcode per page. 
  > It does not include the time taken to load/decode an image (Tiff, PNG, etc) from disk into memory.

  <br>

Some advanced parameters are not listed. See [C++ PublicRuntimeSettings](https://www.dynamsoft.com/barcode-reader/programming/c-cplusplus/struct/PublicRuntimeSettings.html?src=cpp&&ver=latest) for more info.

