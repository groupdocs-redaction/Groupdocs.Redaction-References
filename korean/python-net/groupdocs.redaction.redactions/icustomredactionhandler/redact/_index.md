---
title: "redact 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "특정 문서 내용에 사용자 정의 삭제를 적용합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

특정 문서 내용에 사용자 정의 삭제를 적용합니다.

현재, 이는 PDF에만 지원됩니다 [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

사용자는 AI 기반 편집과 같이 자체적인 편집 로직을 정의할 수 있으며, 이는 단순한 패턴 기반 방법보다 더 고급일 수 있습니다.

```python
def redact(self, context):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| context | `CustomRedactionContext` | 관련 메타데이터와 함께 편집될 문서 내용을 포함합니다. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### 또 보기
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
