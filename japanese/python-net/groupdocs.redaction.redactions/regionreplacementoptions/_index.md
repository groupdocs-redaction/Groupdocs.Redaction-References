---
title: "RegionReplacementOptions クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "画像領域置換のための色と領域パラメータを表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

画像領域置換のための色と領域パラメータを表します。

詳しく読む：
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

RegionReplacementOptions 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | 新しい RegionReplacementOptions インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | サイズが指定されたテキストに一致する RegionReplacementOptions クラスの新しいインスタンスを初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | 編集領域を塗りつぶすために使用される色です。 |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | 矩形の幅と高さです。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # 置換する領域の左上位置を定義します
    point = Point(516, 311)
    # 置換する領域のサイズを定義します
    size = Size(170, 35)
    # 置換として実線の黒い矩形を使用します
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`RegionReplacementOptions` を使用するタスクガイド:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
