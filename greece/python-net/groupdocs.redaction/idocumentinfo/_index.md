---
title: "IDocumentInfo κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει τις απαιτούμενες μεθόδους για την λήψη βασικών πληροφοριών εγγράφου."
type: docs
url: /el/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Παρέχει τις απαιτούμενες μεθόδους για την λήψη βασικών πληροφοριών εγγράφου.

Μάθετε περισσότερα: Λήψη πληροφοριών αρχείου (https://docs.groupdocs.com/redaction/net/get-file-info/).

Ο τύπος IDocumentInfo εκθέτει τα ακόλουθα μέλη:

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Η περιγραφή μορφής αρχείου. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Το συνολικό πλήθος σελίδων. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Η λίστα των αντικειμένων [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) που αντιπροσωπεύουν πληροφορίες σελίδας. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Το μέγεθος του εγγράφου σε byte. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Δείτε επίσης
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
