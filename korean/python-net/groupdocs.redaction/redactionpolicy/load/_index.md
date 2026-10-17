---
title: "load 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "XML 파일에서 RedactionPolicy를 로드합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

XML 파일에서 RedactionPolicy를 로드합니다.

```python
def load(cls, file_path):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_path | `str` | XML 파일 경로입니다. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 예제

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

XML 구성을 포함하는 스트림에서 RedactionPolicy 인스턴스를 로드합니다.

```python
def load(cls, input):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| input | `io.RawIOBase` | XML 구성을 포함하는 스트림입니다. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### 예제

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# XML 파일에서 정책을 로드합니다
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# 문서에 정책을 적용합니다
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### 또 보기
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
