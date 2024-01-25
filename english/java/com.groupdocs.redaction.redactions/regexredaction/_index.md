---
title: RegexRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a text redaction that searches and replaces text in the document by matching provided regular expression.
type: docs
weight: 26
url: /java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Represents a text redaction that searches and replaces text in the document by matching provided regular expression.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document text redactions: [Text redactions][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Text redactions]: https://docs.groupdocs.com/redaction/java/text-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of RegexRedaction class. |
| [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of RegexRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getRegularExpression()](#getRegularExpression--) | Gets the regular expression to match. |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Initializes a new instance of RegexRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Initializes a new instance of RegexRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Gets the regular expression to match.

**Returns:**
java.util.regex.Pattern - The regular expression to match.
### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
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
