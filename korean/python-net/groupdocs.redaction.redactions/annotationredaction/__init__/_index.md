---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "정규식 패턴과 교체 텍스트를 사용하여 새로운 AnnotationRedaction을 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

정규식 패턴과 교체 텍스트를 사용하여 새로운 AnnotationRedaction을 초기화합니다.

```python
def __init__(self, pattern, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| pattern | `str` | 일치시킬 정규식. |
| replacement | `str` | 일치하는 텍스트에 대한 텍스트 교체. |

### 예제

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 주석 텍스트에서 "approved" 단어를 가리기
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

새 인스턴스를 초기화합니다 [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/).

```python
def __init__(self, regex, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 일치시킬 정규식. |
| replacement | `str` | 일치하는 텍스트에 대한 텍스트 교체. |

### 예제

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# 대소문자를 구분하지 않고 "approved" 단어를 가리고 "[REVIEW]" 로 교체하기
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### 또 보기
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
