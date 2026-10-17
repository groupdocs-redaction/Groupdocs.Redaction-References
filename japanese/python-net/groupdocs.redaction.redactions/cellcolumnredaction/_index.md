---
title: "CellColumnRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "スプレッドシートドキュメント（CSV、Excel など）のテキストを置換するテキストレダクションを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

スプレッドシートドキュメント（CSV、Excel など）のテキストを置換するテキストレダクションを表します。

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

CellColumnRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | 新しい CellColumnRedaction を初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | リダクションの説明で、名前とパラメータが含まれます。 |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | 列とワークシートのフィルターです。 |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | 一致させる正規表現パターンです。 |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | テキスト置換のタイプを指定する [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) インスタンス。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | グラフィックコンテンツからテキストを抽出するために使用される IOcrConnector 実装。（[`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) から継承） |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
