---
title: com.groupdocs.redaction.options
second_title: GroupDocs.Redaction for Java API Reference
description: The package provides load and save options classes.
type: docs
weight: 15
url: /java/com.groupdocs.redaction.options/
---

The package provides load and save options classes.


## Classes

| Class | Description |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | Provides options that will be used to open a file. |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | Provides options to sets requirements and stream delegates for preview generation. |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | Provides options for converting files into PDF. |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | Represents redaction settings, allowing to customize the redaction process. |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | Provides options for changing an output file name and/or converting the document to image-based PDF (rasterization). |

## Interfaces

| Interface | Description |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | Provides method that returns a stream to write page preview data. |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | Defines interface of a logger that can be used for logging events and errors in process of redaction. |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | Represents a method which releases stream created by  CreatePageStream  delegate. |

## Enumerations

| Enum | Description |
| --- | --- |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | Represents a list of supported PDF compliance levels. |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | Represents supported preview formats. |
