---
title: "PdfComplianceLevel"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "サポートされている PDF 準拠レベルの一覧を表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.redaction.options/pdfcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum PdfComplianceLevel extends Enum<PdfComplianceLevel>
```

サポートされている PDF 準拠レベルの一覧を表します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Auto](#Auto) | 出力ファイルはデフォルトで PDF/A-1b 標準に準拠します。 |
|
|  | [PdfA1a](#PdfA1a) | 出力ファイルは PDF/A-1a 標準に準拠します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Auto {#Auto}
```
public static final PdfComplianceLevel Auto
```


出力ファイルはデフォルトで PDF/A-1b 標準に準拠します。


### PdfA1a {#PdfA1a}
```
public static final PdfComplianceLevel PdfA1a
```


出力ファイルは PDF/A-1a 標準に準拠します。


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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel)
