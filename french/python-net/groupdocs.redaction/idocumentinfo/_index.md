---
title: "IDocumentInfo classe"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit les méthodes nécessaires pour obtenir les informations de base du document."
type: docs
url: /fr/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Fournit les méthodes nécessaires pour obtenir les informations de base du document.

En savoir plus : Obtenir les informations du fichier (https://docs.groupdocs.com/redaction/net/get-file-info/).

Le type IDocumentInfo expose les membres suivants :

### Propriétés
| Propriété | Description |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | La description du format de fichier. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Le nombre total de pages. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | La liste des objets [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) représentant les informations de page. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | La taille du document en octets. |

### Exemple

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Voir aussi
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
