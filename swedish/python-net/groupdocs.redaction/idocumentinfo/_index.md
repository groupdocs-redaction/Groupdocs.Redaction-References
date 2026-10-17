---
title: "IDocumentInfo klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillhandahåller metoder som krävs för att hämta grundläggande dokumentinformation."
type: docs
url: /sv/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Tillhandahåller metoder som krävs för att hämta grundläggande dokumentinformation.

Läs mer: Hämta filinformation (https://docs.groupdocs.com/redaction/net/get-file-info/).

IDocumentInfo-typen visar följande medlemmar:

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Filformatbeskrivningen. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Det totala sidantalet. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Listan över [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) objekt som representerar sidinformation. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Dokumentets storlek i byte. |

### Exempel

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Se även
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
