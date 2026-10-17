---
title: "get_document_info Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Ruft allgemeine Informationen über das Dokument ab, wie Größe und Seitenanzahl."
type: docs
url: /de/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Ruft allgemeine Informationen über das Dokument ab, wie Größe und Seitenanzahl.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Beispiel

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Siehe auch
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
