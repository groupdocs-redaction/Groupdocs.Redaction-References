---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "모든 주석을 삭제하도록 설정된 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다(모두 일치)."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

모든 주석을 삭제하도록 설정된 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다(모두 일치).

```python
def __init__(self):
    ...
```

### 예제

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 모든 주석 삭제
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

주어진 표현식과 일치하는 주석을 삭제하는 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, pattern):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| pattern | `str` | 정규식. |

### 예제

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 단어 "internal"이 포함된 주석을 삭제합니다(대소문자 구분 없음).
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

주어진 표현식과 일치하는 주석을 삭제하는 DeleteAnnotationRedaction 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, regex):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | 정규식. |

### 예제

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# 내용이 정규식과 일치하는 주석 삭제 (대소문자 구분 없음)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### 또 보기
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
