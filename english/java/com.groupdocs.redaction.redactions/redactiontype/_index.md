---
title: RedactionType
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a type of documents data affected by redaction.
type: docs
weight: 34
url: /java/com.groupdocs.redaction.redactions/redactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionType extends Enum<RedactionType>
```

Represents a type of document's data, affected by redaction.
## Fields

| Field | Description |
| --- | --- |
| [Text](#Text) | The document's body text. |
| [Metadata](#Metadata) | The document's metadata. |
| [Annotation](#Annotation) | The annotations within document's text. |
| [ImageArea](#ImageArea) | The area within an image. |
| [Page](#Page) | The page of a document. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Text {#Text}
```
public static final RedactionType Text
```


The document's body text.

### Metadata {#Metadata}
```
public static final RedactionType Metadata
```


The document's metadata.

### Annotation {#Annotation}
```
public static final RedactionType Annotation
```


The annotations within document's text.

### ImageArea {#ImageArea}
```
public static final RedactionType ImageArea
```


The area within an image.

### Page {#Page}
```
public static final RedactionType Page
```


The page of a document.

### values() {#values--}
```
public static RedactionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionType valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[RedactionType](../../com.groupdocs.redaction.redactions/redactiontype)
