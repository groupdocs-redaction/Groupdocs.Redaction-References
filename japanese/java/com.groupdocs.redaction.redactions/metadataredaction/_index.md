---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "ドキュメントのメタデータ削除のための基本抽象クラスを表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

ドキュメントのメタデータ削除のための基本抽象クラスを表します。

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFilter()](#getFilter--) | すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタを取得します。 |
|
|  | [setFilter(int value)](#setFilter-int-) | すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタを設定します。 |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 指定されたフォーマットインスタンスにレダクションを適用します。 |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタを取得します。


**Returns:**
int - すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタ。

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタを設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | int | すべてまたは特定のメタデータ（例：AuthorやCompany）を選択するために使用されるフィルタ。 |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


指定されたフォーマットインスタンスにレダクションを適用します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | レダクションを適用するドキュメントのインスタンス |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

