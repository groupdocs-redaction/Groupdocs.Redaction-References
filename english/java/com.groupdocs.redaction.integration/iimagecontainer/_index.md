---
title: IImageContainer
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required to access an array of images e.g.
type: docs
weight: 20
url: /java/com.groupdocs.redaction.integration/iimagecontainer/
---```
public interface IImageContainer
```

Defines methods that are required to access an array of images (e.g. embedded within a document) to apply redactions.
## Methods

| Method | Description |
| --- | --- |
| [loadImages()](#loadImages--) | Loads an array of raster image instances, implementing  IImageFormatInstance , contained within the document. |
### loadImages() {#loadImages--}
```
public abstract IImageFormatInstance[] loadImages()
```


Loads an array of raster image instances, implementing  IImageFormatInstance , contained within the document.

**Returns:**
com.groupdocs.redaction.integration.IImageFormatInstance[] - An array of raster image instances
