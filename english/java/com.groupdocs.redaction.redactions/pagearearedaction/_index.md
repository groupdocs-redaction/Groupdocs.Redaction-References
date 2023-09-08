---
title: PageAreaRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a complex textual redaction that affects text images and annotations in an area of the page.
type: docs
weight: 21
url: /java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

Represents a complex textual redaction that affects text, images and annotations in an area of the page.

--------------------

**Learn more**

 *  More details about document metadata redactions: [Redaction basics][]
 *  More details about PageAreaRedaction: [Use PageAreaRedaction][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Use PageAreaRedaction]: https://docs.groupdocs.com/redaction/java/use-page-area-redaction/
## Constructors

| Constructor | Description |
| --- | --- |
| [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of PageAreaRedaction class. |
| [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Initializes a new instance of PageAreaRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getImageOptions()](#getImageOptions--) | Gets the  RegionReplacementOptions  options with color and area parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


Initializes a new instance of PageAreaRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


Initializes a new instance of PageAreaRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |
| imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Replacement options (image area) |

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


Gets the  RegionReplacementOptions  options with color and area parameters.

**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.
### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applies the redaction to a given format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any
