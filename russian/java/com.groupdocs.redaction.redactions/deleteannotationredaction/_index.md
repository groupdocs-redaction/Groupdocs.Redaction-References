---
title: "DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет редактирование текста, которое удаляет аннотации, если текст соответствует заданному регулярному выражению, опционально удаляя все аннотации."
type: docs
weight: 15
url: /ru/java/com.groupdocs.redaction.redactions/deleteannotationredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class DeleteAnnotationRedaction extends Redaction
```

Представляет текстовое редактирование, которое удаляет аннотации, если текст соответствует заданному регулярному выражению (по желанию удаляет все аннотации).

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](../https://docs.groupdocs.com/redaction/java/annotation-redactions/)

<br />

Следующий пример демонстрирует, как удалить все аннотации, содержащие слова "use", "show" или "describe", из документа (и оставить остальные).

````

  try (Redactor redactor = new Redactor("D:\\test.docx"))
 {
    redactor.apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
    redactor.save()
 }
 
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
| [DeleteAnnotationRedaction()](#DeleteAnnotationRedaction--) | Initializes a new instance of DeleteAnnotationRedaction class, with settings to delete all annotations (matching everything).
 |
| [DeleteAnnotationRedaction(String pattern)](#DeleteAnnotationRedaction-java.lang.String-) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.
 |
| [DeleteAnnotationRedaction(Pattern regex)](#DeleteAnnotationRedaction-java.util.regex.Pattern-) | Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.
 |
## Methods

| Method | Description |
| --- | --- |
| [getExpression()](#getExpression--) | Gets the regular expression to match.
 |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters.
 |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance.
 |
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
| pattern | java.lang.String | Regular expression
 |

### DeleteAnnotationRedaction(Pattern regex) {#DeleteAnnotationRedaction-java.util.regex.Pattern-}
```
public DeleteAnnotationRedaction(Pattern regex)
```


Initializes a new instance of DeleteAnnotationRedaction class, deleting annotations matching given expression.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression
 |

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
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction
 |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

