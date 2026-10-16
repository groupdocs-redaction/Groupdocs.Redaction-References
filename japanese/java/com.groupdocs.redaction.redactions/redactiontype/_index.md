---
title: "RedactionType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "マスク処理によって影響を受ける文書データのタイプを表します。"
type: docs
weight: 27
url: /ja/java/com.groupdocs.redaction.redactions/redactiontype/
---
**Inheritance:**
java.lang.Object
```
public final class RedactionType
```

削除の影響を受けるドキュメントデータのタイプを表します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Text](#Text) | 文書の本文テキスト。 |
|
|  | [Metadata](#Metadata) | 文書のメタデータ。 |
|
|  | [Annotation](#Annotation) | 文書テキスト内の注釈。 |
|
|  | [ImageArea](#ImageArea) | 画像内の領域。 |
|
|  | [Page](#Page) | 文書のページ。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [values()](#values--) | RedactionType 値のリスト。 |
|
### Text {#Text}
```
public static final int Text
```


文書の本文テキスト。


### Metadata {#Metadata}
```
public static final int Metadata
```


文書のメタデータ。


### Annotation {#Annotation}
```
public static final int Annotation
```


文書テキスト内の注釈。


### ImageArea {#ImageArea}
```
public static final int ImageArea
```


画像内の領域。


### Page {#Page}
```
public static final int Page
```


文書のページ。


### values() {#values--}
```
public static List<String> values()
```


RedactionType 値のリスト。


**Returns:**
java.util.List<java.lang.String>
