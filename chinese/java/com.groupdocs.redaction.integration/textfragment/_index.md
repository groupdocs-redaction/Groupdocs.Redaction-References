---
title: "TextFragment"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示由 OCR 引擎提取的已识别文本、单词、符号等的一部分。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

表示由 OCR 引擎提取的已识别文本的一部分（单词、符号等）。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | 初始化已识别文本片段的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getText()](#getText--) | 获取已识别文本片段的文本内容。 |
|
|  | [getRectangle()](#getRectangle--) | 获取已识别文本片段的边界矩形。 |
|
|  | [toString()](#toString--) | 返回已识别文本片段的文本内容。 |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


初始化已识别文本片段的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文本 | java.lang.String | 已识别文本片段的文本内容 |
|
|  | rectangle | java.awt.Rectangle | 已识别文本片段的边界矩形 |
|

### getText() {#getText--}
```
public final String getText()
```


获取已识别文本片段的文本内容。


**Returns:**
java.lang.String - 已识别文本片段的文本内容。

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


获取已识别文本片段的边界矩形。


**Returns:**
java.awt.Rectangle - 已识别文本片段的边界矩形。

### toString() {#toString--}
```
public String toString()
```


返回已识别文本片段的文本内容。


**Returns:**
java.lang.String - 已识别文本片段的文本内容

