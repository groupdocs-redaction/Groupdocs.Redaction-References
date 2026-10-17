---
title: "get_document_info metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Hämtar allmän information om dokumentet, såsom storlek och sidantal."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Hämtar allmän information om dokumentet, såsom storlek och sidantal.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Exempel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Se även
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
