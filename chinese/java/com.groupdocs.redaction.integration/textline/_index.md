---
title: "TextLine"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示由 OCR 引擎从图像中提取的文本行。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

表示由 OCR 引擎从图像中提取的一行文本。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | 初始化由 OCR 引擎从图像中提取的文本行的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFragments()](#getFragments--) | 获取该行中识别的文本片段数组，例如符号和单词。 |
|
|  | [toString()](#toString--) | 返回已识别文本行的文本内容。 |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


初始化由 OCR 引擎从图像中提取的文本行的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | 初始文本片段集合 |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


获取该行中识别的文本片段数组，例如符号和单词。


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - 该行中识别的文本片段数组，例如符号和单词。

### toString() {#toString--}
```
public String toString()
```


返回已识别文本行的文本内容。


**Returns:**
java.lang.String - 已识别文本行的文本内容

