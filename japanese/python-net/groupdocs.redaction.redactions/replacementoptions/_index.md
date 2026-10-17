---
title: "ReplacementOptions クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "一致したテキスト置換のオプションを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

一致したテキスト置換のオプションを表します。

詳細を見る

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

ReplacementOptions 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | 指定された置換テキストで ReplacementOptions の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | オプションとしてカラー矩形を使用して ReplacementOptions クラスの新しいインスタンスを初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | 置換アクション: ボックスを描画するかテキストを置換するか。 |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | `ReplacementType.draw_box` オプションの色（それ以外は無視されます）。 |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | ユーザーが独自のレダクションロジックを定義できるカスタムレダクションハンドラ。 |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | このレダクションで適用するフィルタの配列。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | テキスト置換値。 |

### 例

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 一致したテキストをプレースホルダー "[X]" に置換する
repl_opt = ReplacementOptions("[X]")
```

### Guides
`ReplacementOptions` を使用するタスクガイド:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
