---
title: "AnnotationRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "指定された正規表現に一致するアノテーションテキスト（コメントなど）を置換するレダクションを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

指定された正規表現に一致するアノテーションテキスト（コメントなど）を置換するレダクションを表します。

詳細を見る

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

AnnotationRedaction タイプは次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | 正規表現パターンと置換テキストを使用して新しい AnnotationRedaction を初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) の新しいインスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | レダクションの説明で、レダクションとそのパラメータを記述します。 |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | 一致させる正規表現です。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | 一致したテキストのテキスト置換。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
`AnnotationRedaction` を使用するタスクガイド：

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
