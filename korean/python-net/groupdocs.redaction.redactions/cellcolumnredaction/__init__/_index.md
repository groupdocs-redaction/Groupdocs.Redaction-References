---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "새 CellColumnRedaction을 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#filter-reg_ex-options}

새 CellColumnRedaction을 초기화합니다.

```python
def __init__(self, filter, reg_ex, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| filter | `CellFilter` | 열 및 워크시트 필터. |
| reg_ex | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| options | `ReplacementOptions` | 교체 옵션. |

### 예제

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

### 또 보기
* class [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/)
