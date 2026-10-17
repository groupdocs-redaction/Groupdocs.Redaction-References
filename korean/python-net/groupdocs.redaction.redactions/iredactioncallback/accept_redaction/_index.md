---
title: "accept_redaction 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서에 대한 모든 삭제를 적용하기 직전에 트리거되어 로깅하거나 이를 금지할 수 있습니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

문서에 대한 모든 삭제를 적용하기 직전에 트리거되어 로깅하거나 이를 금지할 수 있습니다.

```python
def accept_redaction(self, description):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| description | `RedactionDescription` | 특정 매치 유형, 기준, 텍스트 및 위치에 대한 정보를 포함합니다. |

**Returns:** bool: True to accept the redaction, False to decline it.

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### 또 보기
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
