---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "새로운 RegionReplacementOptions 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#fill_color-size}

새로운 RegionReplacementOptions 인스턴스를 초기화합니다.

```python
def __init__(self, fill_color, size):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 영역을 채우는 색상. |
| size | `System.Drawing.Size` | 채워진 영역 크기. |

### 예제

```python
from groupdocs.redaction.redactions import RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

options = RegionReplacementOptions(Color.BLACK, Size(200, 80))
```

## __init__ {#fill_color-font-expected_text}

주어진 텍스트에 맞는 크기의 RegionReplacementOptions 클래스 새 인스턴스를 초기화합니다.

```python
def __init__(self, fill_color, font, expected_text):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| fill_color | `System.Drawing.Color` | 영역을 채우는 색상. |
| font | `System.Drawing.Font` | 예상 텍스트 폰트. |
| expected_text | `str` | 예상 텍스트. |

### 또 보기
* class [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/)
