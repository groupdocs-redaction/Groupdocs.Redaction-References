---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "새 RemovePageRedaction을 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#origin-index-count}

새 RemovePageRedaction을 초기화합니다.

```python
def __init__(self, origin, index, count):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| origin | `PageSeekOrigin` | 문서의 시작 또는 끝인 기준 위치를 찾습니다. |
| index | `int` | 시작 위치 인덱스 (0 기반). |
| count | `int` | 제거할 페이지 수. |

### 예제

```python
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# 두 번째 페이지(인덱스 1)부터 시작하여 3페이지를 제거합니다.
redaction = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)
```

### 또 보기
* class [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/)
