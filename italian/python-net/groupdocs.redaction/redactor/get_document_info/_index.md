---
title: "metodo get_document_info"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Recupera le informazioni generali sul documento, come dimensione e numero di pagine."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Recupera le informazioni generali sul documento, come dimensione e numero di pagine.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Genera | Descrizione |
| :- | :- |
| `PasswordRequiredException` | Generato quando il documento è protetto da password. |
| `IncorrectPasswordException` | Generato quando viene fornita una password non valida. |

### Esempio

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Vedi anche
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
