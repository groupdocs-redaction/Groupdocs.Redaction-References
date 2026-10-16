---
title: "PdfComplianceLevel"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示受支持的 PDF 合规级别列表。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.redaction.options/pdfcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum PdfComplianceLevel extends Enum<PdfComplianceLevel>
```

表示受支持的 PDF 合规级别列表。

## 字段

| 字段 | 描述 |
| --- | --- |
|  | [Auto](#Auto) | 默认情况下，输出文件将符合 PDF/A-1b 标准。 |
|
|  | [PdfA1a](#PdfA1a) | 输出文件将符合 PDF/A-1a 标准。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Auto {#Auto}
```
public static final PdfComplianceLevel Auto
```


默认情况下，输出文件将符合 PDF/A-1b 标准。


### PdfA1a {#PdfA1a}
```
public static final PdfComplianceLevel PdfA1a
```


输出文件将符合 PDF/A-1a 标准。


### values() {#values--}
```
public static PdfComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.PdfComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static PdfComplianceLevel valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel)
