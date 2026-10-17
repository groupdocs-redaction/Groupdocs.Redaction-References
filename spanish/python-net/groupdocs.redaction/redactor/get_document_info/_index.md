---
title: "método get_document_info"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Recupera la información general del documento, como el tamaño y el número de páginas."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Recupera la información general del documento, como el tamaño y el número de páginas.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Lanza | Descripción |
| :- | :- |
| `PasswordRequiredException` | Se lanza cuando el documento está protegido con contraseña. |
| `IncorrectPasswordException` | Se lanza cuando se proporciona una contraseña inválida. |

### Ejemplo

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Ver también
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
