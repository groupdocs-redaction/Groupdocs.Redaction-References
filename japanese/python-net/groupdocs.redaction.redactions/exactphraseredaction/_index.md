---
title: "ExactPhraseRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントのテキスト内の正確なフレーズを置換するテキストレダクションを表します（デフォルトで大文字小文字を区別しません）。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

ドキュメントのテキスト内の正確なフレーズを置換するテキストレダクションを表します（デフォルトで大文字小文字を区別しません）。

詳しく読む：
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | 大文字小文字を区別しないモードで ExactPhraseRedaction の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | 新しい ExactPhraseRedaction インスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | リダクションの名前とパラメータを含む、リダクションの説明です。 |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | 検索が大文字小文字を区別するかどうかを示す値です。 |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | テキストが右から左へかどうかを示すテキスト方向フラグです。デフォルトは False です。 |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | 検索および置換する文字列です。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | テキスト置換のタイプを指定する [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) インスタンス。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | グラフィックコンテンツからテキストを抽出するために使用される IOcrConnector 実装。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # 大文字小文字を区別した置換
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
`ExactPhraseRedaction` を使用するタスク ガイド:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
