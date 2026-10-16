---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ワードプロセッシング ドキュメントの OOXML 準拠レベル。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

ワードプロセッシング文書の OOXML 準拠レベルです。Strict は Transitional のみへダウングレードでき、Ecma へはダウングレードできません。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 第1版、2006年。 |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional。 |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 第1版、2006年。


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
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
