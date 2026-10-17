---
title: "IDocumentInfo Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt die für das Abrufen grundlegender Dokumentinformationen erforderlichen Methoden bereit."
type: docs
url: /de/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Stellt die für das Abrufen grundlegender Dokumentinformationen erforderlichen Methoden bereit.

Erfahren Sie mehr: Dateiinformationen abrufen (https://docs.groupdocs.com/redaction/net/get-file-info/).

Der IDocumentInfo-Typ stellt die folgenden Mitglieder bereit:

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Die Dateiformatbeschreibung. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Die Gesamtseitenzahl. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Die Liste der [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) Objekte, die Seiteninformationen darstellen. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Die Dokumentgröße in Bytes. |

### Beispiel

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Siehe auch
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
