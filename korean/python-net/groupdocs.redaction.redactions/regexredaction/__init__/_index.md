---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "RegexRedaction의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/regexredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-options}

RegexRedaction의 새 인스턴스를 초기화합니다.

```python
def __init__(self, pattern, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| pattern | `str` | 검색 및 교체를 위한 정규식. |
| options | `ReplacementOptions` | 교체 옵션 (텍스트, 색상). |

### 예제

```python
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

## __init__ {#regex-options}

새 RegexRedaction 인스턴스를 초기화합니다.

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
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

redaction = RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]"))
```

### 또 보기
* class [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)
