---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ワードプロセッシングの保存オプション。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

ワードプロセッシングの保存オプション。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | 保存時に適用する OOXML 準拠。 |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


保存時に適用する OOXML 準拠。null は元のドキュメントレベルを保持します。Strict は直接 Ecma として保存できないため、まず Transitional を使用してください。


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

