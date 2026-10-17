---
title: "get_document_info μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Ανακτά γενικές πληροφορίες για το έγγραφο, όπως το μέγεθος και τον αριθμό σελίδων."
type: docs
url: /el/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

Ανακτά γενικές πληροφορίες για το έγγραφο, όπως το μέγεθος και τον αριθμό σελίδων.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Δείτε επίσης
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
