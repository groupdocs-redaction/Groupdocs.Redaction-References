---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "지정된 교체 텍스트를 사용하여 ReplacementOptions의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#replacement}

지정된 교체 텍스트를 사용하여 ReplacementOptions의 새 인스턴스를 초기화합니다.

```python
def __init__(self, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| replacement | `str` | 텍스트 교체. |

### 예제

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 일치하는 텍스트를 "[REDACTED]" 로 교체
options = ReplacementOptions("[REDACTED]")
```

## __init__ {#color}

색상 사각형을 옵션으로 하여 ReplacementOptions 클래스의 새 인스턴스를 초기화합니다:

```python
def __init__(self, color):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| color | `System.Drawing.Color` | 사각형 색상. |

### 또 보기
* class [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/)
