---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "文字处理文档的 OOXML 合规级别。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

用于文字处理文档的 OOXML 合规级别。Strict 只能降级为 Transitional，不能降级为 Ecma。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 第1版，2006 年。 |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional。 |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 第1版，2006 年。


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional。


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict。


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
