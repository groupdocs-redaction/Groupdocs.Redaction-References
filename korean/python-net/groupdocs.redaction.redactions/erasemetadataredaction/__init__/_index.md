---
title: "__init__ 생성자"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "EraseMetadataRedaction 클래스의 새 인스턴스를 초기화하여 모든 메타데이터를 삭제합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

EraseMetadataRedaction 클래스의 새 인스턴스를 초기화하여 모든 메타데이터를 삭제합니다.

```python
def __init__(self):
    ...
```

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

EraseMetadataRedaction의 새 인스턴스를 초기화하고, 지정된 `MetadataFilters`와 일치하는 메타데이터를 지웁니다.

```python
def __init__(self, filter):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| filter | `MetadataFilters` | 지울 메타데이터를 필터링합니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # 모든 메타데이터 지우기
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # 작성자 메타데이터 필드만 지웁니다.
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### 또 보기
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
