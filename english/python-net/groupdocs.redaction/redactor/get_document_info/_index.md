---
title: get_document_info method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Retrieves the general information about the document, such as size and page count."
type: docs
url: /python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Retrieves the general information about the document, such as size and page count.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Raises | Description |
| :- | :- |
| `PasswordRequiredException` | Raised when the document is password protected. |
| `IncorrectPasswordException` | Raised when an invalid password is provided. |

### Example

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
