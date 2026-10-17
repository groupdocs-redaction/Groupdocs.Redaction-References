---
title: "PageInfo Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine kurze Seiteninformation dar."
type: docs
url: /de/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Stellt eine kurze Seiteninformation dar.

Mehr erfahren:
- https://docs.groupdocs.com/redaction/net/get-file-info/

Der PageInfo-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | Die Seitenhöhe. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Die Seitennummer. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | Die Seitenbreite. |

### Beispiel

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

### Siehe auch
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
