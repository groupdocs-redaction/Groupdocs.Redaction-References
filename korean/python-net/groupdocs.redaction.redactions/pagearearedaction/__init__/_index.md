---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "새로운 PageAreaRedaction 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#regex-options}

새로운 PageAreaRedaction 인스턴스를 초기화합니다.

```python
def __init__(self, regex, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| options | `ReplacementOptions` | 교체 옵션 (텍스트, 색상). |

### 예제

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

새로운 PageAreaRedaction을 초기화합니다.

```python
def __init__(self, regex, options, image_options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| options | `ReplacementOptions` | 교체 옵션 (텍스트, 색상). |
| image_options | `RegionReplacementOptions` | 교체 옵션 (이미지 영역). |

### 예제

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

### 또 보기
* class [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/)
