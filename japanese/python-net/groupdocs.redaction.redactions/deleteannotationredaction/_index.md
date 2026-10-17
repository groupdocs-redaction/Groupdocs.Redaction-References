---
title: "DeleteAnnotationRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "テキストが指定された正規表現に一致した場合にアノテーションを削除するテキストレダクションを表します（オプションで全アノテーションを削除）。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

テキストが指定された正規表現に一致した場合にアノテーションを削除するテキストレダクションを表します（オプションで全アノテーションを削除）。

詳細を見る

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

DeleteAnnotationRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | すべてのアノテーション（すべてに一致）を削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | 指定された式に一致するアノテーションを削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | 指定された式に一致するアノテーションを削除する設定で、DeleteAnnotationRedaction クラスの新しいインスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | リダクションの名前とパラメータを含む、リダクションの説明です。 |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | 一致させる正規表現です。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # 単語 "internal" を含むアノテーションを削除（大文字小文字を区別しない）
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
`DeleteAnnotationRedaction` を使用するタスク ガイド:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
