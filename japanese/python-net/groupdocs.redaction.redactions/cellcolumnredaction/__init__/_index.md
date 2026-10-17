---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "新しい CellColumnRedaction を初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

新しい CellColumnRedaction を初期化します。

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| filter | `CellFilter` | 列とワークシートのフィルタ。 |
| reg_ex | `System.Text.RegularExpressions.Regex` | 検索と置換に使用する正規表現。 |
| options | `ReplacementOptions` | 置換オプション。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("spreadsheet.xlsx") as redactor:
    redactor.apply(
        CellColumnRedaction(
            CellFilter(worksheet="Sheet1", column=2),
            r"\bsecret\b",
            ReplacementOptions(Color.BLACK)
        )
    )
    redactor.save()
```

### 関連項目
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
