---
title: "get_document_info 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서의 크기 및 페이지 수와 같은 일반 정보를 검색합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

문서의 크기 및 페이지 수와 같은 일반 정보를 검색합니다.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### 예제

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### 또 보기
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
