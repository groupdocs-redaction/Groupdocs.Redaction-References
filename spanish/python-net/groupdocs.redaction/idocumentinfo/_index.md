---
title: "Clase IDocumentInfo"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Proporciona los métodos necesarios para obtener información básica del documento."
type: docs
url: /es/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Proporciona los métodos necesarios para obtener información básica del documento.

Más información: Obtener información del archivo (https://docs.groupdocs.com/redaction/net/get-file-info/).

El tipo IDocumentInfo expone los siguientes miembros:

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | La descripción del formato de archivo. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | El recuento total de páginas. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | La lista de objetos [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) que representan la información de la página. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | El tamaño del documento en bytes. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Ver también
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
