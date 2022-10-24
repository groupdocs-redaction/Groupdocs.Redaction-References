---
title: SaveOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Provides options for changing an output file name and/or converting the document to image-based PDF rasterization.
type: docs
weight: 14
url: /java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Provides options for changing an output file name and/or converting the document to image-based PDF (rasterization).

--------------------

**Learn more**

 *  [Save with default options][]
 *  [Save in rasterized PDF][]
 *  [Select specific pages for rasterized PDF][]
 *  [Save in original format][]
 *  [Save overwriting original file][]
 *  [Save to stream][]


[Save with default options]: https://docs.groupdocs.com/redaction/java/save-with-default-options/
[Save in rasterized PDF]: https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/
[Select specific pages for rasterized PDF]: https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/
[Save in original format]: https://docs.groupdocs.com/redaction/java/save-in-original-format/
[Save overwriting original file]: https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/
[Save to stream]: https://docs.groupdocs.com/redaction/java/save-to-stream/
## Constructors

| Constructor | Description |
| --- | --- |
| [SaveOptions()](#SaveOptions--) | Initializes a new instance with defaults: rasterize to PDF - false, add suffix - false. |
| [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Initializes a new instance with given parameters. |
## Fields

| Field | Description |
| --- | --- |
| [SaveSuffix](#SaveSuffix) | Represents default suffix value, which is "Redacted". |
## Methods

| Method | Description |
| --- | --- |
| [getAddSuffix()](#getAddSuffix--) | Gets a value indicating whether the file name needs to be changed before saving. |
| [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Sets a value indicating whether the file name needs to be changed before saving. |
| [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Gets a custom suffix for output file name. |
| [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Sets a custom suffix for output file name. |
| [getRasterizeToPDF()](#getRasterizeToPDF--) | Gets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |
| [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |
| [getRasterization()](#getRasterization--) | Gets the rasterization settings. |
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Initializes a new instance with defaults: rasterize to PDF - false, add suffix - false.

### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Initializes a new instance with given parameters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rasterizeToPdf | boolean | True, if all pages in the document need to be converted to images and put in a single PDF file |
| suffix | java.lang.String | This text will be added to the end of file name, if not empty also sets AddSuffix to true |

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Represents default suffix value, which is "Redacted".

### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Gets a value indicating whether the file name needs to be changed before saving. False by default.

**Returns:**
boolean - A value indicating whether the file name needs to be changed before saving. False by default.
### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Sets a value indicating whether the file name needs to be changed before saving. False by default.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether the file name needs to be changed before saving. False by default. |

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Gets a custom suffix for output file name. If it is not specified, the  SaveSuffix  constant will be used.

**Returns:**
java.lang.String - A custom suffix for output file name. If it is not specified, the  SaveSuffix  constant will be used.
### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Sets a custom suffix for output file name. If it is not specified, the  SaveSuffix  constant will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A custom suffix for output file name. If it is not specified, the  SaveSuffix  constant will be used. |

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Gets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file.

**Returns:**
boolean - A value indicating whether all pages in the document need to be converted to images and put in a single PDF file.
### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Gets the rasterization settings.

**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.
