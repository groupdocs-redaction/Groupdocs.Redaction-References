---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一种文本编辑，默认情况下在文档文本中不区分大小写地替换确切短语。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

表示一种文本编辑，默认情况下不区分大小写地替换文档文本中的确切短语。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

以下示例演示了执行区分大小写的短语搜索和替换。

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// 默认情况下，isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | 在不区分大小写模式下初始化 ExactPhraseRedaction 类的新实例。 |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | 初始化 ExactPhraseRedaction 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | 获取要搜索和替换的字符串。 |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | 获取一个值，指示搜索是否区分大小写。 |
|
|  | [isRightToLeft()](#isRightToLeft--) | 获取一个值，指示此文本是否从右到左，默认 false。 |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | 设置一个值，指示此文本是否从右到左，默认 false。 |
|
|  | [getDescription()](#getDescription--) | 返回一个字符串，描述 redaction 及其参数。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 将 redaction 应用于给定的格式实例。 |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


在不区分大小写模式下初始化 ExactPhraseRedaction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 要搜索和替换的字符串 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 替换选项（文本，颜色） |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


初始化 ExactPhraseRedaction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 要搜索和替换的字符串 |
|
|  | isCaseSensitive | boolean | 如果需要区分大小写的搜索，则为 True |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 替换选项（文本，颜色） |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


获取要搜索和替换的字符串。


**Returns:**
java.lang.String - 要搜索和替换的字符串。

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


获取一个值，指示搜索是否区分大小写。


**Returns:**
boolean - 一个值，指示搜索是否区分大小写。

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


获取一个值，指示此文本是否从右到左，默认 false。


**Returns:**
boolean - 一个值，指示此文本是否从右到左，默认 false。

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


设置一个值，指示此文本是否从右到左，默认 false。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 一个值，指示此文本是否从右到左，默认 false。 |
|

### getDescription() {#getDescription--}
```
public String getDescription()
```


返回一个字符串，描述 redaction 及其参数。


**Returns:**
java.lang.String - 包含 redaction 名称和参数的文本。

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


将 redaction 应用于给定的格式实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 用于应用 redaction 的文档实例 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

