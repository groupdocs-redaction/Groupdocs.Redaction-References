---
title: PageInfo class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a brief page information."
type: docs
url: /python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Represents a brief page information.

Learn more:
- https://docs.groupdocs.com/redaction/net/get-file-info/

The PageInfo type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Properties
| Property | Description |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | The page height. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | The page number. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | The page width. |

### Example

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
