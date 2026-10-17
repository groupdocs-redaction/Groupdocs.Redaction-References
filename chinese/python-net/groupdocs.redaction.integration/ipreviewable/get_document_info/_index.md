---
title: "get_document_info 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "检索文档的一般信息，例如大小和页数。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/ipreviewable/get_document_info/
is_root: false
weight: 1030
---


## get_document_info

检索文档的一般信息，例如大小和页数。

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing file type, page count, size, and pages.

### 示例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### 另请参阅
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
