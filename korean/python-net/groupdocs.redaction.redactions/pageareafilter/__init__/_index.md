---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "특정 영역을 가리기 위해 새로운 PageAreaFilter를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/
is_root: false
weight: 10
---


## __init__ {#top_left-size}

특정 영역을 가리기 위해 새로운 PageAreaFilter를 초기화합니다.

```python
def __init__(self, top_left, size):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| top_left | `System.Drawing.Point` | 좌상단 영역 좌표. |
| size | `System.Drawing.Size` | 영역 크기 및 색상. |

### 예제

```python
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

point = Point(0, 100)
size = Size(200, 150)
filter = PageAreaFilter(point, size)
```

### 또 보기
* class [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/)
