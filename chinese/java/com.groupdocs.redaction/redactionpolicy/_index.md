---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一个包含一组特定要执行的编辑的清理策略。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

表示一个清理策略，包含一组要应用的特定编辑。

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | 创建 Redaction 策略的新实例。 |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | 使用特定的编辑列表创建 Redaction 策略的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | 获取完全配置好的数组 |
编辑
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | 加载一个实例 |
RedactionPolicy
来自文件路径。
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | 加载一个实例 |
RedactionPolicy
来自流。
|
|  | [save(String filePath)](#save-java.lang.String-) | 将 redaction 策略保存到文件。 |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | 将 redaction 策略保存到流。 |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


创建 Redaction 策略的新实例。


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


使用特定的编辑列表创建 Redaction 策略的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | 策略的编辑数组 |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


获取完全配置好的数组
编辑
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - 完全配置好的 Redaction 派生类数组。

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


加载一个实例
RedactionPolicy
来自文件路径。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | XML 文件的路径 |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


加载一个实例
RedactionPolicy
来自流。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 输入 | java.io.InputStream | 包含 XML 配置的流 |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


将 redaction 策略保存到文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 文件路径。 |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


将 redaction 策略保存到流。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 输出 | java.io.OutputStream | 用于保存策略的目标流 |
|

