---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "特定の矩形領域を赤字化するための新しい ImageAreaRedaction を初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

特定の矩形領域を赤字化するための新しい ImageAreaRedaction を初期化します。

```python
def __init__(self, top_left, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 左上領域の座標。 |
| options | `RegionReplacementOptions` | 領域のサイズと色。 |

### 例

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# マスクする領域の左上隅を定義する
top_left = Point(385, 485)
# マスク領域のサイズと色を定義する
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# マスクオブジェクトを作成する
redaction = ImageAreaRedaction(top_left, region_options)
```

### 関連項目
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
