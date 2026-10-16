---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示通过匹配提供的正则表达式搜索并替换文档中文本的文本编辑。"
type: docs
weight: 28
url: /zh/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

表示通过匹配提供的正则表达式搜索并替换文档中文本的文本编辑。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | 初始化 RegexRedaction 类的新实例。 |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | 初始化 RegexRedaction 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | 获取要匹配的正则表达式。 |
|
|  | [getDescription()](#getDescription--) | 返回一个字符串，描述 redaction 及其参数。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 将 redaction 应用于给定的格式实例。 |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


初始化 RegexRedaction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 模式 | java.lang.String | 用于搜索和替换的正则表达式 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 替换选项（文本，颜色） |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


初始化 RegexRedaction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 正则表达式 | java.util.regex.Pattern | 用于搜索和替换的正则表达式 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 替换选项（文本，颜色） |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


获取要匹配的正则表达式。


**Returns:**
java.util.regex.Pattern - 用于匹配的正则表达式。

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

