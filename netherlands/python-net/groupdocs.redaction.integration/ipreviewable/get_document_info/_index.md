---
title: "get_document_info methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Haalt algemene informatie over het document op, zoals grootte en paginatelling."
type: docs
url: /nl/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Haalt algemene informatie over het document op, zoals grootte en paginatelling.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Voorbeeld

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Zie ook
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
