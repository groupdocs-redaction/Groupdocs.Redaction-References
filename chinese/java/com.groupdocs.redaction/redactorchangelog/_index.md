---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示传递给 Redactor 类的 Apply 方法的编辑列表的结果。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

表示传递给 Apply() 方法的编辑列表的结果，
Redactor
类。

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | 初始化 RedactorChangeLog 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 获取所有已应用编辑的最终状态。 |
|
|  | [getRedactionLog()](#getRedactionLog--) | 获取列表的 |
RedactorLogEntry
实例。
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


初始化 RedactorChangeLog 类的新实例。


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


获取所有已应用编辑的最终状态。


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


获取列表的
RedactorLogEntry
实例。


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - RedactorLogEntry 实例的列表。

