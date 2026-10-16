---
title: "TextReplacement"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示文本替换信息。"
type: docs
weight: 33
url: /zh/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

表示文本替换信息。

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | 初始化 TextReplacement 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getIndex()](#getIndex--) | 获取匹配文本在源字符串中的索引。 |
|
|  | [getOriginalText()](#getOriginalText--) | 获取原始匹配的字符串。 |
|
|  | [getReplacement()](#getReplacement--) | 获取字符串，替换 OriginalText。 |
|
|  | [toString()](#toString--) | 提供文本替换描述及其位置。 |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


初始化 TextReplacement 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 索引 | int | 源字符串中匹配文本的索引 |
|
|  | 原始 | java.lang.String | 原始匹配字符串 |
|
|  | 替换 | java.lang.String | 字符串，在源字符串中替换 OriginalText |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


获取匹配文本在源字符串中的索引。


**Returns:**
int - 源字符串中匹配文本的索引。

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


获取原始匹配的字符串。


**Returns:**
java.lang.String - 原始匹配字符串。

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


获取字符串，替换 OriginalText。


**Returns:**
java.lang.String - 替换 OriginalText 的字符串。

### toString() {#toString--}
```
public String toString()
```


提供文本替换描述及其位置。


**Returns:**
java.lang.String - 替换描述

