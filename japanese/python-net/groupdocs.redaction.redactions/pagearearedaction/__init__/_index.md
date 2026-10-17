---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "新しい PageAreaRedaction インスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

新しい PageAreaRedaction インスタンスを初期化します。

```python
def __init__(self, regex, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[SSN]"))
    )
    redactor.save()
```

## __init__ {#regex-options-image_options}

新しい PageAreaRedaction を初期化します。

```python
def __init__(self, regex, options, image_options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション（テキスト、色）。 |
| image_options | `RegionReplacementOptions` | 置換オプション（画像領域）。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

redactor = Redactor("scan.pdf")
redactor.apply(
    PageAreaRedaction(
        r"\d{3}-\d{2}-\d{4}",
        ReplacementOptions("[SSN]"),
        RegionReplacementOptions(Color.BLACK, Size(120, 20))
    )
)
redactor.save()
```

### 関連項目
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
