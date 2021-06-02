---
layout: default-layout
title: Dynamsoft Barcode Reader JavaScript API Reference - BarcodeReader
description: This page shows the BarcodeReader Class of Dynamsoft Barcode Reader JavaScript SDK.
keywords: TextResult, BarcodeReader, api reference, javascript, js
needAutoGenerateSidebar: false
breadcrumbText: TextResult
---

Dynamsoft Barcode Reader SDK - JavaScript API
# TextResult

`interface` TextResult

* barcodeText: *string*

  > The barcode text.

* barcodeFormat: *number | [EnumBarcodeFormat](../enum/EnumBarcodeFormat.md)*

  > The barcode format.

* barcodeFormatString: *string*

  > Barcode type in string.

* barcodeBytes: *number[]*

  > The barcode content in a byte array.

* localizationResult: *[LocalizationResult](LocalizationResult.md)*

  > The corresponding localization result.

```js
let reader = await Dynamsoft.DBR.BarcodeReader.createInstance();
let results = await reader.decode(imageSource);
for(let result of results){
  console.log(result.barcodeText);
}
```

Some advanced parameters are not listed. See [C++ TextResult](https://www.dynamsoft.com/barcode-reader/programming/c-cplusplus/struct/TextResult.html?src=cpp&&ver=latest) for more info.