---
title: "RegexRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト赤字を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

提供された正規表現に一致させてドキュメント内のテキストを検索・置換するテキスト赤字を表します。

詳細を見る

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

RegexRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | RegexRedaction の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | 新しい RegexRedaction インスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | リダクションの説明で、名前とパラメータが含まれます。 |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | マッチングに使用される正規表現パターン。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | テキスト置換のタイプを指定する [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) インスタンス。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | グラフィックコンテンツからテキストを抽出するために使用される IOcrConnector 実装。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # テキストで置換
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # 青い実線矩形で置換
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
`RegexRedaction` を使用するタスクガイド:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
