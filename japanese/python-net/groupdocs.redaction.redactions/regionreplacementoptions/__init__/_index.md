---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "新しい RegionReplacementOptions インスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

新しい RegionReplacementOptions インスタンスを初期化します。

```python
def __init__(self, fill_color, size):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 領域を塗りつぶす色。 |
| size | `System.Drawing.Size` | 塗りつぶされた領域のサイズ。 |

### 例

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

サイズが指定されたテキストに一致する RegionReplacementOptions クラスの新しいインスタンスを初期化します。

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 領域を塗りつぶす色。 |
| font | `System.Drawing.Font` | 期待されるテキストフォント。 |
| expected_text | `str` | 期待されるテキスト。 |

### 関連項目
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
