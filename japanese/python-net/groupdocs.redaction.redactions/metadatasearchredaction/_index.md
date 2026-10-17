---
title: "MetadataSearchRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "正規表現を使用してキーや値を一致させ、メタデータを検索・赤字化するメタデータ赤字を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

正規表現を使用してキーや値を一致させ、メタデータを検索・赤字化するメタデータ赤字を表します。

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | MetadataSearchRedaction クラスの新しいインスタンスを初期化し、値を使用して削除された項目と一致させます。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | MetadataSearchRedaction の新しいインスタンスを初期化し、項目名と値を使用して削除された項目と一致させます。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | MetadataSearchRedaction クラスの新しいインスタンスを初期化し、値を使用して削除された項目と一致させます。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | MetadataSearchRedaction の新しいインスタンスを初期化し、項目名と値を使用して削除された項目と一致させます。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | 指定されたフォーマットインスタンスに赤字処理を適用します。(継承元: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (継承元: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | リダクションの説明で、名前とパラメータが含まれます。 |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | メタデータ項目の名前（キー）に一致させる正規表現です。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | テキスト置換値。 |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | メタデータ項目の値テキストに一致させる正規表現です。 |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Author や Company など、すべてまたは特定のメタデータを選択するために使用されるフィルタです。(継承元: [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # パターンに一致するメタデータ値をすべて削除します。
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
`MetadataSearchRedaction` を使用するタスク ガイド:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
