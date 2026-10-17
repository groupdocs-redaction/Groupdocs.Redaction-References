---
title: "result 속성"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "DocumentFormatInstance가 반환한 결과."
type: docs
url: /ko/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)에 의해 반환된 결과입니다.

모든 메타데이터 편집은 각 메타데이터 항목에 별도로 적용되며, 메타데이터 항목 편집이 실패하더라도 나머지 메타데이터 항목은 업데이트됩니다. 실패하거나 건너뛴(거부된) 메타데이터 항목 및 그 이유 목록은 `ErrorMessage` 속성의 [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/)에서 확인할 수 있습니다.

### Definition:
```python
@property
def result(self):
    ...
```

### 또 보기
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
