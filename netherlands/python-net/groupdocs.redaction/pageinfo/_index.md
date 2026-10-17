---
title: "PageInfo klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een korte paginainformatie voor."
type: docs
url: /nl/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Stelt een korte paginainformatie voor.

Meer informatie:
- https://docs.groupdocs.com/redaction/net/get-file-info/

Het PageInfo-type bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | De paginahoogte. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Het paginanummer. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | De paginabreedte. |

### Voorbeeld

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

### Zie ook
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
