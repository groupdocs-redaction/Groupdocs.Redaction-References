---
title: "groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "groupdocs.redaction.redactions の型です。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


`groupdocs.redaction.redactions` の型。

### クラス
| クラス | 説明 |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | 指定された正規表現に一致するアノテーションテキスト（コメントなど）を置換するレダクションを表します。 |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | スプレッドシートドキュメント（CSV、Excel など）のテキストを置換するテキストレダクションを表します。 |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) の対象範囲をワークシートと列に限定するオプションを提供します。 |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | カスタムレダクション処理のコンテキストを提供します。 |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | カスタムレダクション操作の結果を表します。 |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | テキストが指定された正規表現に一致した場合にアノテーションを削除するテキストレダクションを表します（オプションで全アノテーションを削除）。 |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | ドキュメントからすべてのメタデータまたは特定の MetadataFilters に一致するメタデータを消去するメタデータレダクションを表します。 |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | ドキュメントのテキスト内の正確なフレーズを置換するテキストレダクションを表します（デフォルトで大文字小文字を区別しません）。 |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | カスタムレダクションロジックを実装するためのインターフェイスを提供します。 |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | 各赤字変更に関する情報を受け取るために必要なメソッドを定義し、必要に応じてそれを防止します。 |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | 画像ドキュメントの指定領域にカラーの長方形を配置する赤字を表します。 |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | ドキュメントメタデータの赤字処理のための基底抽象クラスを表します。 |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | 正規表現を使用してキーや値を一致させ、メタデータを検索・赤字化するメタデータ赤字を表します。 |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | ドキュメントのページ内の領域を設定し、赤字を適用する赤字フィルターを表します。 |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | ページの領域内のテキスト、画像、注釈に影響を与える複合的なテキスト赤字を表します。 |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | ドキュメント内のページ範囲を設定し、赤字を適用する赤字フィルターを表します。 |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | 赤字処理中に実行された単一の変更アクション情報を表します。 |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | 提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト赤字を表します。 |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | 画像領域置換のための色と領域パラメータを表します。 |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | ドキュメントからページ（スライド、ワークシート等）を削除する赤字を表します。 |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | 一致したテキスト置換のオプションを表します。 |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | ドキュメントテキスト赤字のための基底抽象クラスを表します。 |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | テキスト置換情報を表します。 |

### 列挙型
| 列挙体 | 説明 |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | ドキュメント内の適用範囲を設定し、赤字を適用する赤字フィルターを表します。 |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
