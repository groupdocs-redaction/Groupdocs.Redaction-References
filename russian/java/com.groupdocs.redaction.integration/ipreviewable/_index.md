---
title: "IPreviewable"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Определяет методы для создания предварительного просмотра документа."
type: docs
weight: 25
url: /ru/java/com.groupdocs.redaction.integration/ipreviewable/
---```
public interface IPreviewable
```

Defines methods to create preview of the document.

## Methods

| Method | Description |
| --- | --- |
| [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Generates preview images of specific pages in a given image format.
 |
| [getDocumentInfo()](#getDocumentInfo--) | Gets the general information about the document - size, page count, etc.
 |
### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public abstract void generatePreview(PreviewOptions previewOptions)
```


Generates preview images of specific pages in a given image format.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Image properties and page range settings
 |

### getDocumentInfo() {#getDocumentInfo--}
```
public abstract IDocumentInfo getDocumentInfo()
```


Gets the general information about the document - size, page count, etc.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

