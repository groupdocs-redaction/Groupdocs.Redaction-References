---
title: "classe IDocumentInfo"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Fornisce i metodi necessari per ottenere informazioni di base sul documento."
type: docs
url: /it/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Fornisce i metodi necessari per ottenere informazioni di base sul documento.

Maggiori informazioni: Ottieni informazioni sul file (https://docs.groupdocs.com/redaction/net/get-file-info/).

Il tipo IDocumentInfo espone i seguenti membri:

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | La descrizione del formato file. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Il conteggio totale delle pagine. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | L'elenco degli oggetti [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) che rappresentano le informazioni della pagina. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | La dimensione del documento in byte. |

### Esempio

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Vedi anche
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
