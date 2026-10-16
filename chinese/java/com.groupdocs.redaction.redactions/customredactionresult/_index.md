---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示由 . 返回的结果。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

表示由 [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) 返回的结果。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getApply()](#getApply--) | 获取一个值，指示是否应应用替换。 |
|
|  | [setApply(boolean value)](#setApply-boolean-) | 设置一个值，指示是否应应用替换。 |
|
|  | [getText()](#getText--) | 获取在 #getApply().getApply() 为时使用的替换文本 |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | 设置在 #getApply().getApply() 为时使用的替换文本 |
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


获取一个值，指示是否应应用替换。


**Returns:**
boolean -  true  用于将匹配的文本替换为 #getText().getText(); 否则为  false 。

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


设置一个值，指示是否应应用替换。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | true  用于应用替换；否则为  false 。 |
|

### getText() {#getText--}
```
public final String getText()
```


获取在 #getApply().getApply() 为时使用的替换文本
true
.


**Returns:**
java.lang.String - 替换文本。

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


设置在 #getApply().getApply() 为时使用的替换文本
true
.


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 替换文本。 |
|

