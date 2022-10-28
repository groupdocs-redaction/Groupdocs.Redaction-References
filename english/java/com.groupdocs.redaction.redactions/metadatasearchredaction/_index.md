---
title: MetadataSearchRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a metadata redaction that searches and redacts metadata using regular expressions matching keys and/or values.
type: docs
weight: 19
url: /java/com.groupdocs.redaction.redactions/metadatasearchredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.MetadataRedaction](../../com.groupdocs.redaction.redactions/metadataredaction)
```
public class MetadataSearchRedaction extends MetadataRedaction
```

Represents a metadata redaction that searches and redacts metadata using regular expressions, matching keys and/or values.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document metadata redactions: [Metadata redactions][]

The following example demonstrates how to search and redact certain text in specific metadata.

```

  try (Redactor redactor = new Redactor("C:\\sample.docx"))
 {
    MetadataSearchRedaction redaction = new MetadataSearchRedaction("Company Ltd.", "--company--");
    // If not set, applies to all metadata items
    redaction.setFilter( MetadataFilters.Company );
    redactor.apply(redaction);
    redactor.save();
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Metadata redactions]: https://docs.groupdocs.com/redaction/java/metadata-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [MetadataSearchRedaction(String valuePattern, String replacement)](#MetadataSearchRedaction-java.lang.String-java.lang.String-) | Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items. |
| [MetadataSearchRedaction(String valuePattern, String replacement, String keyPattern)](#MetadataSearchRedaction-java.lang.String-java.lang.String-java.lang.String-) | Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items. |
| [MetadataSearchRedaction(Pattern valueRegex, String replacement)](#MetadataSearchRedaction-java.util.regex.Pattern-java.lang.String-) | Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items. |
| [MetadataSearchRedaction(Pattern valueRegex, String replacement, Pattern keyRegex)](#MetadataSearchRedaction-java.util.regex.Pattern-java.lang.String-java.util.regex.Pattern-) | Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items. |
## Methods

| Method | Description |
| --- | --- |
| [getValueExpression()](#getValueExpression--) | Gets the regular expression to match value text of a metadata item. |
| [getReplacement()](#getReplacement--) | Gets the textual replacement value. |
| [getKeyExpression()](#getKeyExpression--) | Gets the regular expression to match name (key) of metadata item. |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
### MetadataSearchRedaction(String valuePattern, String replacement) {#MetadataSearchRedaction-java.lang.String-java.lang.String-}
```
public MetadataSearchRedaction(String valuePattern, String replacement)
```


Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valuePattern | java.lang.String | Regular expression to search and replace |
| replacement | java.lang.String | Textual replacement |

### MetadataSearchRedaction(String valuePattern, String replacement, String keyPattern) {#MetadataSearchRedaction-java.lang.String-java.lang.String-java.lang.String-}
```
public MetadataSearchRedaction(String valuePattern, String replacement, String keyPattern)
```


Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valuePattern | java.lang.String | Regular expression to search and replace metadata item value |
| replacement | java.lang.String | Textual replacement |
| keyPattern | java.lang.String | Regular expression to search and replace metadata item name |

### MetadataSearchRedaction(Pattern valueRegex, String replacement) {#MetadataSearchRedaction-java.util.regex.Pattern-java.lang.String-}
```
public MetadataSearchRedaction(Pattern valueRegex, String replacement)
```


Initializes a new instance of MetadataSearchRedaction class, using value to match redacted items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueRegex | java.util.regex.Pattern | Regular expression to search and replace |
| replacement | java.lang.String | Textual replacement |

### MetadataSearchRedaction(Pattern valueRegex, String replacement, Pattern keyRegex) {#MetadataSearchRedaction-java.util.regex.Pattern-java.lang.String-java.util.regex.Pattern-}
```
public MetadataSearchRedaction(Pattern valueRegex, String replacement, Pattern keyRegex)
```


Initializes a new instance of MetadataSearchRedaction class, using item name and value to match redacted items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueRegex | java.util.regex.Pattern | Regular expression to search and replace metadata item value |
| replacement | java.lang.String | Textual replacement |
| keyRegex | java.util.regex.Pattern | Regular expression to search and replace metadata item name |

### getValueExpression() {#getValueExpression--}
```
public final Pattern getValueExpression()
```


Gets the regular expression to match value text of a metadata item.

**Returns:**
java.util.regex.Pattern - The regular expression to match value text of a metadata item.
### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Gets the textual replacement value.

**Returns:**
java.lang.String - The textual replacement value.
### getKeyExpression() {#getKeyExpression--}
```
public final Pattern getKeyExpression()
```


Gets the regular expression to match name (key) of metadata item.

**Returns:**
java.util.regex.Pattern - The regular expression to match name (key) of metadata item.
### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
