---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "대소문자 구분 없이 ExactPhraseRedaction의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#search_phrase-options}

대소문자 구분 없이 ExactPhraseRedaction의 새 인스턴스를 초기화합니다.

```python
def __init__(self, search_phrase, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| search_phrase | `str` | 검색 및 교체할 문자열. |
| options | `ReplacementOptions` | 교체 옵션 (텍스트, 색상). |

### 예제

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 대소문자를 구분하지 않고 "John Doe"를 "[CUSTOMER]" 로 교체하기
redaction = ExactPhraseRedaction("John Doe", ReplacementOptions("[CUSTOMER]"))
```

## __init__ {#search_phrase-is_case_sensitive-options}

새 ExactPhraseRedaction 인스턴스를 초기화합니다.

```python
def __init__(self, search_phrase, is_case_sensitive, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| search_phrase | `str` | 검색 및 교체할 문자열. |
| is_case_sensitive | `bool` | 대소문자를 구분하는 검색이 필요한 경우 True. |
| options | `ReplacementOptions` | 교체 옵션 (텍스트, 색상). |

### 예제

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 대소문자 구분 없는 정확한 구문 가리기
redaction = ExactPhraseRedaction("John Doe", False, ReplacementOptions("[CUSTOMER]"))

# 대소문자 구분 정확한 구문 가리기
redaction_cs = ExactPhraseRedaction("ACME", True, ReplacementOptions("[CO]"))
```

### 또 보기
* class [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/)
