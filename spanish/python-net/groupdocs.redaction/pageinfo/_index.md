---
title: "Clase PageInfo"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa información breve de la página."
type: docs
url: /es/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Representa información breve de la página.

Más información:
- https://docs.groupdocs.com/redaction/net/get-file-info/

El tipo PageInfo expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | La altura de la página. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | El número de página. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | El ancho de la página. |

### Ejemplo

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

### Ver también
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
