---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "특정 사각형 영역을 가리기 위한 새 ImageAreaRedaction을 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-options}

특정 사각형 영역을 가리기 위한 새 ImageAreaRedaction을 초기화합니다.

```python
def __init__(self, top_left, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 좌상단 영역 좌표. |
| options | `RegionReplacementOptions` | 영역 크기 및 색상. |

### 예제

```python
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

# 가리기 영역의 좌상단 모서리를 정의합니다
top_left = Point(385, 485)
# 가리기 영역의 크기와 색상을 정의합니다
region_options = RegionReplacementOptions(Color.from_argb(255, 220, 20, 60), Size(1793, 2069))

# 가리기 객체를 생성합니다
redaction = ImageAreaRedaction(top_left, region_options)
```

### 또 보기
* class [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/)
