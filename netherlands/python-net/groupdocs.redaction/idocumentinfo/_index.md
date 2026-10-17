---
title: "IDocumentInfo klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt methoden die nodig zijn om basisdocumentinformatie op te halen."
type: docs
url: /nl/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Biedt methoden die nodig zijn om basisdocumentinformatie op te halen.

Meer informatie: Get file info (https://docs.groupdocs.com/redaction/net/get-file-info/).

Het IDocumentInfo-type geeft de volgende leden weer:

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | De beschrijving van het bestandsformaat. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Het totale aantal pagina's. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | De lijst met [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) objecten die paginainformatie weergeven. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | De documentgrootte in bytes. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Zie ook
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
