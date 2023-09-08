---
title: IFixedFormatDocument
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for access formats of fixed structure such as PDF or presentations.
type: docs
weight: 19
url: /java/com.groupdocs.redaction.integration/ifixedformatdocument/
---```
public interface IFixedFormatDocument
```

Defines methods that are required for access formats of fixed structure, such as PDF or presentations.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about PageAreaRedaction: [Use PageAreaRedaction][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Use PageAreaRedaction]: https://docs.groupdocs.com/redaction/java/use-page-area-redaction/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [redactAnnotation(Pattern regularExpression, ReplacementOptions options)](#redactAnnotation-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Replaces the matching text in all annotations within the document with given options. |
| [loadImages(RedactionFilter[] filters)](#loadImages-com.groupdocs.redaction.redactions.RedactionFilter---) | Loads an array of raster image instances, contained within the document, matching  Redactions.RedactionFilter  set. |
### redactAnnotation(Pattern regularExpression, ReplacementOptions options) {#redactAnnotation-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public abstract RedactionResult redactAnnotation(Pattern regularExpression, ReplacementOptions options)
```


Replaces the matching text in all annotations within the document with given options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Replacement result
### loadImages(RedactionFilter[] filters) {#loadImages-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public abstract IImageFormatInstance[] loadImages(RedactionFilter[] filters)
```


Loads an array of raster image instances, contained within the document, matching  Redactions.RedactionFilter  set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | An array of RedactionFilter instances to apply |

**Returns:**
com.groupdocs.redaction.integration.IImageFormatInstance[] - An array of raster image instances
