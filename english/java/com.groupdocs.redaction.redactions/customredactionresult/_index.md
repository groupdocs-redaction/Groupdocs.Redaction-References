---
title: CustomRedactionResult
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a result returned by .
type: docs
weight: 14
url: /java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Represents a result returned by [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructors

| Constructor | Description |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getApply()](#getApply--) | Gets a value indicating whether the replacement should be applied.
 |
| [setApply(boolean value)](#setApply-boolean-) | Sets a value indicating whether the replacement should be applied.
 |
| [getText()](#getText--) | Gets the replacement text used when #getApply().getApply() is 
true
.
 |
| [setText(String value)](#setText-java.lang.String-) | Sets the replacement text used when #getApply().getApply() is 
true
.
 |
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Gets a value indicating whether the replacement should be applied.


**Returns:**
boolean -  true  to replace the matched text with #getText().getText(); otherwise,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Sets a value indicating whether the replacement should be applied.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  true  to apply the replacement; otherwise,  false .
 |

### getText() {#getText--}
```
public final String getText()
```


Gets the replacement text used when #getApply().getApply() is 
true
.


**Returns:**
java.lang.String - The replacement text.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Sets the replacement text used when #getApply().getApply() is 
true
.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The replacement text.
 |

