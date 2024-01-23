---
title: DeleteAnnotationRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a text redaction that deletes annotations if text is matching given regular expression optionally deletes all annotations.
type: docs
weight: 13
url: /java/com.groupdocs.redaction.redactions/deleteannotationredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class DeleteAnnotationRedaction extends Redaction
```

Represents a text redaction that deletes annotations if text is matching given regular expression (optionally deletes all annotations).

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document annotation redactions: [Annotation redactions][]

The following example demonstrates how to remove all annotations containing words "use", "show" or "describe" from document (and leave others).

```

  try (Redactor redactor = new Redactor("D:\\test.docx"))
 {
    redactor.apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
    redactor.save()
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Annotation redactions]: https://docs.groupdocs.com/redaction/java/annotation-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [DeleteAnnotationRedaction()](#DeleteAnnotationRedaction--) | Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything). |
| [DeleteAnnotationRedaction(String pattern)](#DeleteAnnotationRedaction-java.lang.String-) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression. |
| [DeleteAnnotationRedaction(Pattern regex)](#DeleteAnnotationRedaction-java.util.regex.Pattern-) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression. |
## Methods

| Method | Description |
| --- | --- |
| [getExpression()](#getExpression--) | Gets the regular expression to match. |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### DeleteAnnotationRedaction() {#DeleteAnnotationRedaction--}
```
public DeleteAnnotationRedaction()
```


Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything).

### DeleteAnnotationRedaction(String pattern) {#DeleteAnnotationRedaction-java.lang.String-}
```
public DeleteAnnotationRedaction(String pattern)
```


Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | Regular expression |

### DeleteAnnotationRedaction(Pattern regex) {#DeleteAnnotationRedaction-java.util.regex.Pattern-}
```
public DeleteAnnotationRedaction(Pattern regex)
```


Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression |

### getExpression() {#getExpression--}
```
public final Pattern getExpression()
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
