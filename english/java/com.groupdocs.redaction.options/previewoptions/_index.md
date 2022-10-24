---
title: PreviewOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Provides options to sets requirements and stream delegates for preview generation.
type: docs
weight: 11
url: /java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Provides options to sets requirements and stream delegates for preview generation.
## Constructors

| Constructor | Description |
| --- | --- |
| [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Initializes a new instance of PreviewOptions class, causing the output stream to be closed. |
| [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Initializes a new instance of PreviewOptions class, causing the output stream to be returned to the client for further use. |
## Methods

| Method | Description |
| --- | --- |
| [getWidth()](#getWidth--) | Gets or sets page preview width. |
| [setWidth(int value)](#setWidth-int-) | Gets or sets page preview width. |
| [getHeight()](#getHeight--) | Gets or sets page preview height. |
| [setHeight(int value)](#setHeight-int-) | Gets or sets page preview height. |
| [getPageNumbers()](#getPageNumbers--) | Gets or sets an array of page numbers to generate preview. |
| [setPageNumbers(int[] value)](#setPageNumbers-int---) | Gets or sets an array of page numbers to generate preview. |
| [getPreviewFormat()](#getPreviewFormat--) | Gets or sets preview image format. |
| [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Gets or sets preview image format. |
| [getCreatePageStream()](#getCreatePageStream--) | Gets or sets an instance of page stream creation delegate. |
| [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Gets or sets an instance of page stream creation delegate. |
| [getReleasePageStream()](#getReleasePageStream--) | Gets or sets an instance of page preview completion delegate. |
| [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Gets or sets an instance of page preview completion delegate. |
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initializes a new instance of PreviewOptions class, causing the output stream to be closed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Creates a stream for a specific page preview |

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initializes a new instance of PreviewOptions class, causing the output stream to be returned to the client for further use.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Creates a stream for a specific page preview |
| releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Notifies that the page preview generation is done and gets output stream |

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Gets or sets page preview width.

**Returns:**
int - Page preview width.
### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Gets or sets page preview width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Page preview width. |

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Gets or sets page preview height.

**Returns:**
int - Page preview height.
### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Gets or sets page preview height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Page preview height. |

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Gets or sets an array of page numbers to generate preview.

**Returns:**
int[] - An array of page numbers to generate preview.
### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Gets or sets an array of page numbers to generate preview.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int[] | An array of page numbers to generate preview. |

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Gets or sets preview image format.

**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.
### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Gets or sets preview image format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Preview image format. |

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Gets or sets an instance of page stream creation delegate.

**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.
### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Gets or sets an instance of page stream creation delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | An instance of page stream creation delegate. |

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Gets or sets an instance of page preview completion delegate.

**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.
### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Gets or sets an instance of page preview completion delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | An instance of page preview completion delegate. |

