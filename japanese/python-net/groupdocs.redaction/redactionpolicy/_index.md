---
title: "RedactionPolicy クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "適用する特定の編集セットを含むサニタイズ ポリシーを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

適用する特定の編集セットを含むサニタイズ ポリシーを表します。

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

RedactionPolicy 型は次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | 新しい RedactionPolicy インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | 特定の削除リストを使用して新しい RedactionPolicy を初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | XML ファイルから RedactionPolicy をロードします。 |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | XML 設定を含むストリームから RedactionPolicy インスタンスをロードします。 |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | 削除ポリシーをファイルに保存します。 |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | 削除ポリシーをストリームに保存します。 |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | 完全に構成された [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-派生クラスの一覧です。 |

### 例

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# メモリ内で再利用可能なポリシーを構築します
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# ポリシーをドキュメントに適用します
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
`RedactionPolicy` を使用するタスクガイド：

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 関連項目
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
