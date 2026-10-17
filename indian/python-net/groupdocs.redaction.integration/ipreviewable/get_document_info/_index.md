---
title: "get_document_info मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ के बारे में सामान्य जानकारी प्राप्त करता है, जैसे आकार और पृष्ठ संख्या।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

दस्तावेज़ के बारे में सामान्य जानकारी प्राप्त करता है, जैसे आकार और पृष्ठ संख्या।

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### उदाहरण

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### संबंधित देखें
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
