---
title: "metodo get_document_info"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Recupera informazioni generali sul documento, come dimensione e numero di pagine."
type: docs
url: /it/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Recupera informazioni generali sul documento, come dimensione e numero di pagine.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Esempio

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Vedi anche
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
