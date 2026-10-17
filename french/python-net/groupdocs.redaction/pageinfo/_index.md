---
title: "PageInfo classe"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente une brève information de page."
type: docs
url: /fr/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Représente une brève information de page.

En savoir plus :
- https://docs.groupdocs.com/redaction/net/get-file-info/

Le type PageInfo expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Propriétés
| Propriété | Description |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | La hauteur de la page. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Le numéro de la page. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | La largeur de la page. |

### Exemple

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

### Voir aussi
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
