---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示在编辑过程中执行的单个更改操作信息。"
type: docs
weight: 25
url: /zh/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

表示在编辑过程中执行的单个更改操作信息。

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | 初始化 RedactionDescription 类的新实例，不包含替换信息。 |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | 初始化 RedactionDescription 类的新实例，包含替换信息。 |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | 初始化 RedactionDescription 类的新实例，包含图像区域替换信息。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | 获取文档数据的类型 - 文本、元数据或注释。 |
|
|  | [getActionType()](#getActionType--) | 获取编辑操作：替换、清理或删除。 |
|
|  | [getOriginalText()](#getOriginalText--) | 获取匹配的文本（如果提供了表达式）。 |
|
|  | [getReplacement()](#getReplacement--) | 获取替换信息，可能为 null。 |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | 获取图像区域编辑的替换信息，对文本编辑返回 null。 |
|
|  | [getDetails()](#getDetails--) | 获取被编辑项的可选详细信息。 |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | 设置被编辑项的可选详细信息。 |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


初始化 RedactionDescription 类的新实例，不包含替换信息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redactionType | int | 被编辑数据的类型 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 对这些数据要执行的操作 |
|
|  | originalText | java.lang.String | 匹配的文本、注释或标注正文 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


初始化 RedactionDescription 类的新实例，包含替换信息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redactionType | int | 被编辑数据的类型 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 对这些数据要执行的操作 |
|
|  | originalText | java.lang.String | 匹配的文本、注释或标注正文 |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | 替换文本、匹配的文本及其在原始字符串中的位置 |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


初始化 RedactionDescription 类的新实例，包含图像区域替换信息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redactionType | int | 被编辑数据的类型 |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | 对这些数据要执行的操作 |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | 图像区域替换信息 |
|
|  | imageDetails | java.lang.String | 图像文本描述，默认值为 String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


获取文档数据的类型 - 文本、元数据或注释。


**Returns:**
int - 文档数据的类型 - 文本、元数据或标注。

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


获取编辑操作：替换、清理或删除。


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


获取匹配的文本（如果提供了表达式）。


**Returns:**
java.lang.String - 匹配的文本（如果提供了表达式）。

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


获取替换信息，可能为 null。


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


获取图像区域编辑的替换信息，对文本编辑返回 null。


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


获取被编辑项的可选详细信息。


**Returns:**
java.lang.String - 被编辑项的可选详细信息。

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


设置被编辑项的可选详细信息。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 被编辑项的可选详细信息。 |
|

