---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "새 RedactionPolicy 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

새 RedactionPolicy 인스턴스를 초기화합니다.

```python
def __init__(self):
    ...
```

### 예제

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

특정 삭제 목록을 사용하여 새 RedactionPolicy를 초기화합니다.

```python
def __init__(self, redactions):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redactions | `list[Redaction]` | 정책에 대한 redactions 배열. |

### 예제

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### 또 보기
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
