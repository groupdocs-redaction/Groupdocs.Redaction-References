---
title: "طريقة get_document_info"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يسترجع معلومات عامة عن المستند، مثل الحجم وعدد الصفحات."
type: docs
url: /ar/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

يسترجع معلومات عامة عن المستند، مثل الحجم وعدد الصفحات.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### مثال

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### انظر أيضًا
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
