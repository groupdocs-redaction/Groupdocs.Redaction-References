---
title: "classe PageInfo"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta una breve informazione di pagina."
type: docs
url: /it/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Rappresenta una breve informazione di pagina.

Per saperne di più:
- https://docs.groupdocs.com/redaction/net/get-file-info/

Il tipo PageInfo espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | L'altezza della pagina. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Il numero della pagina. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | La larghezza della pagina. |

### Esempio

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

### Vedi anche
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
