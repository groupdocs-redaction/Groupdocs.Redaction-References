---
title: "ImageAreaRedaction クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "画像ドキュメントの指定領域にカラーの長方形を配置する赤字を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

画像ドキュメントの指定領域にカラーの長方形を配置する赤字を表します。

詳しく読む：
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

ImageAreaRedaction 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | 特定の矩形領域を赤字化するための新しい ImageAreaRedaction を初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | 指定されたフォーマット インスタンスに対してリダクションを適用します。 |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | リダクションの説明で、名前とパラメータが含まれます。 |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | 色と領域パラメータを含む RegionReplacementOptions オプション。 |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | 削除する領域の左上位置です。 |

### 例

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`ImageAreaRedaction` を使用するタスク ガイド:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
