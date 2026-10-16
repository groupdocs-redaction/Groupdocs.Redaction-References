---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "このパッケージは、さまざまなタイプの編集（赤字）用クラスを提供します。"
type: docs
weight: 16
url: /ja/java/com.groupdocs.redaction.redactions/
---

このパッケージは、さまざまなタイプの編集（赤字）用クラスを提供します。



## クラス

| クラス | 説明 |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | 指定された正規表現に一致する注釈テキスト（コメントなど）を置換する赤字を表します。 |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | スプレッドシート ドキュメント（CSV、Excel など）のテキストを置換するテキスト赤字を表します。 |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | CellColumnRedaction の対象範囲をワークシートと列に限定するオプションを提供します。 |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) の入力データを提供します。 |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) によって返される結果を表します。 |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | テキストが指定された正規表現に一致する場合に注釈を削除するテキスト赤字を表します（オプションで全ての注釈を削除できます）。 |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | ドキュメントからすべてのメタデータ、または特定の MetadataFilters に一致するメタデータを消去するメタデータ赤字を表します。 |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | デフォルトで大文字小文字を区別せず、ドキュメントのテキスト内の正確なフレーズを置換するテキスト赤字を表します。 |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | 画像ドキュメントの指定領域にカラー矩形を配置する赤字を表します。 |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | 最も一般的なドキュメントメタデータのタイプの一覧を表します。 |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | ドキュメントのメタデータ削除のための基本抽象クラスを表します。 |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | 正規表現を使用してキーや値を一致させ、メタデータを検索および削除するメタデータ削除を表します。 |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | ドキュメントのページ内の領域を設定して削除を適用する削除フィルターを表します。 |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | ページの領域内のテキスト、画像、注釈に影響を与える複合的なテキスト削除を表します。 |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | ドキュメント内のページ範囲を設定して削除を適用する削除フィルターを表します。 |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | 削除プロセス中に実行された単一の変更アクション情報を表します。 |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | ドキュメント内のスコープを設定して削除を適用する削除フィルターを表します。 |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | 削除の影響を受けるドキュメントデータのタイプを表します。 |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | 提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト削除を表します。 |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | 画像領域置換のための色と領域パラメータを表します。 |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | ドキュメントからページ（スライド、ワークシートなど）を削除する削除を表します。 |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | 一致したテキスト置換のオプションを表します。 |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | ドキュメントテキスト削除のための基本抽象クラスを表します。 |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | テキスト置換情報を表します。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | カスタム削除コールバックを定義します。 |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | 各削除変更に関する情報を受け取り、必要に応じてそれを防止するために必要なメソッドを定義します。 |

## 列挙型

| 列挙型 | 説明 |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | シーク用にドキュメント内の参照ポイントを表すフィールドを提供します。 |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | 削除を実行するために取れるアクションを表します。 |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | 一致したテキストの置換タイプを表します。 |
