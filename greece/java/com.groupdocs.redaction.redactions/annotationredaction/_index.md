---
title: "AnnotationRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια διαγραφή που αντικαθιστά κείμενο σχολίων κ.λπ. των σημειώσεων που ταιριάζουν με μια δεδομένη κανονική έκφραση."
type: docs
weight: 10
url: /el/java/com.groupdocs.redaction.redactions/annotationredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class AnnotationRedaction extends Redaction
```

Αντιπροσωπεύει μια επεξεργασία που αντικαθιστά το κείμενο σχολίων (σχόλια κ.λπ.) που ταιριάζει με μια δεδομένη κανονική έκφραση.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](../https://docs.groupdocs.com/redaction/java/annotation-redactions/)

<br />

Το παρακάτω παράδειγμα δείχνει πώς να αντικαταστήσετε το όνομα "John" με "[redacted]" σε όλες τις σημειώσεις.

````

  try (Redactor redactor = new Redactor("C:\\test.pdf"))
 {
    redactor.apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
    redactor.save()
 }
 
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
| [AnnotationRedaction(String pattern, String replacement)](#AnnotationRedaction-java.lang.String-java.lang.String-) | Initializes a new instance of AnnotationRedaction class.
 |
| [AnnotationRedaction(Pattern regex, String replacement)](#AnnotationRedaction-java.util.regex.Pattern-java.lang.String-) | Initializes a new instance of AnnotationRedaction class.
 |
## Methods

| Method | Description |
| --- | --- |
| [getExpression()](#getExpression--) | Gets the regular expression to match.
 |
| [getReplacement()](#getReplacement--) | Gets a textual replacement for matched text.
 |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters.
 |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance.
 |
### AnnotationRedaction(String pattern, String replacement) {#AnnotationRedaction-java.lang.String-java.lang.String-}
```
public AnnotationRedaction(String pattern, String replacement)
```


Initializes a new instance of AnnotationRedaction class.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | Regular expression to match
 |
| replacement | java.lang.String | Textual replacement for matched text
 |

### AnnotationRedaction(Pattern regex, String replacement) {#AnnotationRedaction-java.util.regex.Pattern-java.lang.String-}
```
public AnnotationRedaction(Pattern regex, String replacement)
```


Initializes a new instance of AnnotationRedaction class.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regex | java.util.regex.Pattern | Regular expression to match
 |
| replacement | java.lang.String | Textual replacement for matched text
 |

### getExpression() {#getExpression--}
```
public final Pattern getExpression()
```


Gets the regular expression to match.


**Returns:**
java.util.regex.Pattern - The regular expression to match.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Gets a textual replacement for matched text.


**Returns:**
java.lang.String - A textual replacement for matched text.

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

