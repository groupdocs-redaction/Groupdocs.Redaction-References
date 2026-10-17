---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction 클래스의 새 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, value_pattern, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| value_pattern | `str` | 검색 및 교체에 사용할 정규식 |
| replacement | `str` | 텍스트 교체 |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

항목 이름과 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction의 새 인스턴스를 초기화합니다.

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| value_pattern | `str` | 메타데이터 항목 값을 검색하고 교체하기 위한 정규식. |
| replacement | `str` | 텍스트 교체. |
| key_pattern | `str` | 메타데이터 항목 이름을 검색하고 교체하기 위한 정규식. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # 메타데이터 값에서 발견된 모든 이메일 주소를 교체합니다.
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction 클래스의 새 인스턴스를 초기화합니다.

```python
def __init__(self, value_regex, replacement):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| replacement | `str` | 텍스트 교체. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# 메타데이터에 있는 모든 이메일 주소를 가립니다.
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

항목 이름과 값을 사용하여 삭제된 항목을 일치시키는 MetadataSearchRedaction의 새 인스턴스를 초기화합니다.

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | 메타데이터 항목 값을 검색하고 교체하기 위한 정규식. |
| replacement | `str` | 텍스트 교체. |
| key_regex | `System.Text.RegularExpressions.Regex` | 메타데이터 항목 이름을 검색하고 교체하기 위한 정규식. |

### 예제

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# 메타데이터 값에 있는 이메일 주소를 가립니다.
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### 또 보기
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
