---
title: RasterizationOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Provides options for converting files into PDF.
type: docs
weight: 12
url: /java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Provides options for converting files into PDF.

--------------------

**Learn more**

 *  More details about saving document as a rasterized PDF: [Save in rasterized PDF][]
 *  More details about rasterization options: [Select specific pages for rasterized PDF][]


[Save in rasterized PDF]: https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/
[Select specific pages for rasterized PDF]: https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/
## Constructors

| Constructor | Description |
| --- | --- |
| [RasterizationOptions()](#RasterizationOptions--) | Initializes a new instance. |
## Methods

| Method | Description |
| --- | --- |
| [getEnabled()](#getEnabled--) | Gets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. |
| [getPageIndex()](#getPageIndex--) | Gets the index of the first page (0-based) to convert into PDF. |
| [setPageIndex(int value)](#setPageIndex-int-) | Sets the index of the first page (0-based) to convert into PDF. |
| [isStartPageIndexSet()](#isStartPageIndexSet--) | Gets a value indicating whether the PageIndex property was changed (set) after its initialization. |
| [getPageCount()](#getPageCount--) | Gets the number of pages to be converted into PDF. |
| [setPageCount(int value)](#setPageCount-int-) | Sets the number of pages to be converted into PDF. |
| [isPageCountSet()](#isPageCountSet--) | Gets a value indicating whether the PageCount property was changed (set) after its initialization. |
| [getCompliance()](#getCompliance--) | Gets the PDF Compliance level. |
| [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Sets the PDF Compliance level. |
| [hasAdvancedOptions()](#hasAdvancedOptions--) | Gets an indicator, which is true if advanced rasterization options are set. |
| [addAdvancedOption(int optionType)](#addAdvancedOption-int-) | You can use this method to register an advanced rasterization option to apply. |
| [addAdvancedOption(int optionType, System.Collections.Generic.Dictionary<String,String> parameters)](#addAdvancedOption-int-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--) | You can use this method to register an advanced rasterization option to apply. |
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Initializes a new instance.

### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Gets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization.

**Returns:**
boolean - A value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization.
### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization. |

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Gets the index of the first page (0-based) to convert into PDF.

**Returns:**
int - The index of the first page (0-based) to convert into PDF.
### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Sets the index of the first page (0-based) to convert into PDF.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The index of the first page (0-based) to convert into PDF. |

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Gets a value indicating whether the PageIndex property was changed (set) after its initialization.

**Returns:**
boolean - A value indicating whether the PageIndex property was changed (set) after its initialization.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gets the number of pages to be converted into PDF.

**Returns:**
int - The number of pages to be converted into PDF.
### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Sets the number of pages to be converted into PDF.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The number of pages to be converted into PDF. |

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Gets a value indicating whether the PageCount property was changed (set) after its initialization.

**Returns:**
boolean - A value indicating whether the PageCount property was changed (set) after its initialization.
### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Gets the PDF Compliance level.

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.
### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Sets the PDF Compliance level.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | The PDF Compliance level. |

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Gets an indicator, which is true if advanced rasterization options are set.

**Returns:**
boolean - An indicator, which is true if advanced rasterization options are set.
### addAdvancedOption(int optionType) {#addAdvancedOption-int-}
```
public final void addAdvancedOption(int optionType)
```


You can use this method to register an advanced rasterization option to apply.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| optionType | int | Provides information about the selected effect type (grayscale, border, etc.) |

### addAdvancedOption(int optionType, System.Collections.Generic.Dictionary<String,String> parameters) {#addAdvancedOption-int-com.aspose.ms.System.Collections.Generic.Dictionary-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(int optionType, System.Collections.Generic.Dictionary<String,String> parameters)
```


You can use this method to register an advanced rasterization option to apply.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| optionType | int | Provides information about the selected effect type (grayscale, border, etc.) |
| parameters | com.aspose.ms.System.Collections.Generic.Dictionary<java.lang.String,java.lang.String> | Parameters for the given effect, such as rotation angle |

