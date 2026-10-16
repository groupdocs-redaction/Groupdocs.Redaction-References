---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示从图像中提取的文本，作为识别过程的结果。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

表示从图像中提取的文本，作为其识别过程的结果。

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | 使用一组已识别的行初始化该类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getText()](#getText--) | 获取结构化文本的文本等价。 |
|
|  | [getLines()](#getLines--) | 获取文档中识别的文本行及其片段。 |
|
|  | [toString()](#toString--) | 获取结构化文本的文本等价。 |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


使用一组已识别的行初始化该类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | 已识别行的 IEnumerable（例如列表或数组） |
|

### getText() {#getText--}
```
public final String getText()
```


获取结构化文本的文本等价。


**Returns:**
java.lang.String - 结构化文本的文本等价。

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


获取文档中识别的文本行及其片段。


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - 文档中识别的文本行及其片段。

### toString() {#toString--}
```
public String toString()
```


获取结构化文本的文本等价。


**Returns:**
java.lang.String - 已识别的文本

