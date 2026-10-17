---
title: "PageInfo klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Representerar kort information om en sida."
type: docs
url: /sv/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Representerar kort information om en sida.

Läs mer:
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | Sidans höjd. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Sidnumret. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | Sidbredden. |

### Exempel

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

### Se även
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
