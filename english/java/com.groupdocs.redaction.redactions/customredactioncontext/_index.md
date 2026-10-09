---
title: CustomRedactionContext
second_title: GroupDocs.Redaction for Java API Reference
description: Provides input data for .
type: docs
weight: 13
url: /java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Provides input data for [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructors

| Constructor | Description |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getPageNumber()](#getPageNumber--) | Gets the page number of the matched fragment, when available.
 |
| [setPageNumber(int value)](#setPageNumber-int-) | Sets the page number of the matched fragment.
 |
| [getText()](#getText--) | Gets the text matched for redaction.
 |
| [setText(String value)](#setText-java.lang.String-) | Sets the text matched for redaction.
 |
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Gets the page number of the matched fragment, when available.


**Returns:**
int - The page number, or a format-specific value if the page is not known.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Sets the page number of the matched fragment.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The page number.
 |

### getText() {#getText--}
```
public final String getText()
```


Gets the text matched for redaction.


**Returns:**
java.lang.String - The matched text.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Sets the text matched for redaction.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The matched text.
 |

