---
title: IAnnotatedDocument
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for access to annotations such as comments.
type: docs
weight: 17
url: /java/com.groupdocs.redaction.integration/iannotateddocument/
---```
public interface IAnnotatedDocument
```

Defines methods that are required for access to annotations, such as comments. Needs to be implemented by  DocumentFormatInstance -derived class to perform annotation redactions.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document annotation redactions: [Annotation redactions][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Annotation redactions]: https://docs.groupdocs.com/redaction/java/annotation-redactions/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [redactAnnotation(Pattern regularExpression, String replacement)](#redactAnnotation-java.util.regex.Pattern-java.lang.String-) | Replaces the matching text in all annotations within the document. |
| [deleteAnnotations(Pattern regularExpression)](#deleteAnnotations-java.util.regex.Pattern-) | Deletes all annotations, matching regular expression within the document. |
### redactAnnotation(Pattern regularExpression, String replacement) {#redactAnnotation-java.util.regex.Pattern-java.lang.String-}
```
public abstract RedactionResult redactAnnotation(Pattern regularExpression, String replacement)
```


Replaces the matching text in all annotations within the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace |
| replacement | java.lang.String | Textual replacement |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Replacement result
### deleteAnnotations(Pattern regularExpression) {#deleteAnnotations-java.util.regex.Pattern-}
```
public abstract RedactionResult deleteAnnotations(Pattern regularExpression)
```


Deletes all annotations, matching regular expression within the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to match |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Deletion result
