---
title: "apply 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서에 가리기 작업을 적용합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

문서에 가리기 작업을 적용합니다.

```python
def apply(self, redaction):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redaction | `Redaction` | 적용할 `Redaction` 인스턴스. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### 예제

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # SSN 패턴을 교체하기 위한 redaction을 정의합니다
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # 문서를 로드하고 redaction을 적용합니다
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

문서에 일련의 가리기 작업을 적용합니다.

```python
def apply(self, redactions):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| redactions | `list[Redaction]` | 적용할 redaction 배열 |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### 예제

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataSearchRedaction,
    ReplacementOptions,
)
from groupdocs.redaction.metadata import MetadataFilter

redaction_list = [
    ExactPhraseRedaction("ClientName", ReplacementOptions("[client]")),
    ExactPhraseRedaction("ClientAddress", ReplacementOptions("[address]")),
    RegexRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[ssn]")),
    RegexRedaction(r"\d{16}", ReplacementOptions("[card]")),
    DeleteAnnotationRedaction(r"(?im:(use|show|describe))"),
    EraseMetadataRedaction(MetadataFilter.Author),
    MetadataSearchRedaction("CompanyName", "--company--"),
]

with Redactor("./test.docx") as redactor:
    result = redactor.apply(redaction_list)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#policy}

문서에 가리기 정책을 적용합니다.

```python
def apply(self, policy):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redaction 정책. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### 예제

```python
import os
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import RasterizationOptions

policy = RedactionPolicy.load("RedactionPolicy.xml")
for file_name in os.listdir(r"C:\Inbound"):
    file_path = os.path.join(r"C:\Inbound", file_name)
    with Redactor(file_path) as redactor:
        result = redactor.apply(policy)
        out_folder = (
            r"C:\Outbound\Done"
            if result.status != RedactionStatus.FAILED
            else r"C:\Outbound\Failed"
        )
        out_path = os.path.join(out_folder, file_name)
        with open(out_path, "r+b") as stream:
            redactor.save(stream, RasterizationOptions(enabled=False))
```

### 또 보기
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
