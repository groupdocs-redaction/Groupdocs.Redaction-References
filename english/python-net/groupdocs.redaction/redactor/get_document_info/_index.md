---
title: get_document_info method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Retrieves general information about the document, such as size and page count."
type: docs
url: /python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1040
---


## get_document_info

Retrieves general information about the document, such as size and page count.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: An object containing document size, file type, page count, and page details.

| Raises | Description |
| :- | :- |
| `PasswordRequiredException` | If the document is password protected. |
| `IncorrectPasswordException` | If an invalid password is provided. |

### Example

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Load the document from local disk
    with Redactor("./sample.docx") as redactor:
        info = redactor.get_document_info()
        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")
```

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
