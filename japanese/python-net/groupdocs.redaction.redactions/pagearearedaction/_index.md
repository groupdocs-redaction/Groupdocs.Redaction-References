---
title: "PageAreaRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ページの領域内のテキスト、画像、注釈に影響を与える複合的なテキスト赤字を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

ページの領域内のテキスト、画像、注釈に影響を与える複合的なテキスト赤字を表します。

詳細を見る

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | 新しい PageAreaRedaction インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | 新しい PageAreaRedaction を初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | 色と領域パラメータを含む RegionReplacementOptions オプション。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | テキスト置換のタイプを指定する [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) インスタンス。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | 編集の説明で、名前とパラメータを含みます。（[`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) から継承） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | グラフィックコンテンツからテキストを抽出するために使用される IOcrConnector 実装。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | マッチングに使用される正規表現パターン。（[`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) から継承） |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
