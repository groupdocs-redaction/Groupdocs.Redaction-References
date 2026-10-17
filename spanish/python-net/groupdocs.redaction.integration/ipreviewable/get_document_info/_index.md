---
title: "método get_document_info"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Recupera información general sobre el documento, como el tamaño y el número de páginas."
type: docs
url: /es/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Recupera información general sobre el documento, como el tamaño y el número de páginas.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Ejemplo

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Ver también
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
