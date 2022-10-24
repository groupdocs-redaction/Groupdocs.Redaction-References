---
title: ReplacementType
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a type of replacement for the matched text.
type: docs
weight: 31
url: /java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Represents a type of replacement for the matched text.
## Fields

| Field | Description |
| --- | --- |
| [ReplaceString](#ReplaceString) | Replaces matched text with another string, e.g. |
| [DrawBox](#DrawBox) | Draws a rectangle of specific color (Black by default) instead of redacted text. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Replaces matched text with another string, e.g. exemption code.

### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Draws a rectangle of specific color (Black by default) instead of redacted text.

### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
