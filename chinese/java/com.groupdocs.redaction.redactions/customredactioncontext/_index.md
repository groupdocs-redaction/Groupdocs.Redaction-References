---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "提供输入数据。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

提供输入数据给 [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler)。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | 获取匹配片段的页码（如果可用）。 |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | 设置匹配片段的页码。 |
|
|  | [getText()](#getText--) | 获取用于编辑的匹配文本。 |
|
|  | [setText(String value)](#setText-java.lang.String-) | 设置用于编辑的匹配文本。 |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


获取匹配片段的页码（如果可用）。


**Returns:**
int - 页码，或在未知页码时的特定格式值。

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


设置匹配片段的页码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 页码。 |
|

### getText() {#getText--}
```
public final String getText()
```


获取用于编辑的匹配文本。


**Returns:**
java.lang.String - 匹配的文本。

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


设置用于编辑的匹配文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 匹配的文本。 |
|

