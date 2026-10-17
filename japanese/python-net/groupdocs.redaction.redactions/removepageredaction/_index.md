---
title: "RemovePageRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントからページ（スライド、ワークシート等）を削除する赤字を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

ドキュメントからページ（スライド、ワークシート等）を削除する赤字を表します。

詳細を見る
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | 新しい RemovePageRedaction を初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | 削除するページ数です。 |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | 開始位置インデックス（0 ベース）です。 |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | シーク参照位置で、ドキュメントの先頭または末尾のいずれかです。 |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | リダクションの説明で、名前とパラメータを含みます。( [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/) から継承) |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 文書の末尾から数えて 1 ページを削除します
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # 赤字化を適用します
        result = redactor.apply(rem_opt)

        # 編集されたドキュメントを保存します
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
`RemovePageRedaction` を使用するタスク ガイド:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
