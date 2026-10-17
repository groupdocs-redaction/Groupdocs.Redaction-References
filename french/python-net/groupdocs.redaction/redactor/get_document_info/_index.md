---
title: "méthode get_document_info"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Récupère les informations générales sur le document, telles que la taille et le nombre de pages."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Récupère les informations générales sur le document, telles que la taille et le nombre de pages.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Lève | Description |
| :- | :- |
| `PasswordRequiredException` | Levée lorsque le document est protégé par mot de passe. |
| `IncorrectPasswordException` | Levée lorsqu'un mot de passe invalide est fourni. |

### Exemple

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Voir aussi
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
