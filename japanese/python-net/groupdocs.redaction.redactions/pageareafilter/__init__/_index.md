---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "特定の領域を編集するための新しい PageAreaFilter を初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

特定の領域を編集するための新しい PageAreaFilter を初期化します。

```python
def __init__(self, top_left, size):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 左上領域の座標。 |
| size | `System.Drawing.Size` | 領域のサイズと色。 |

### 例

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### 関連項目
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
