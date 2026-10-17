---
title: "PageInfo κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει σύντομες πληροφορίες σελίδας."
type: docs
url: /el/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Αντιπροσωπεύει σύντομες πληροφορίες σελίδας.

Μάθετε περισσότερα:
- https://docs.groupdocs.com/redaction/net/get-file-info/

Ο τύπος PageInfo εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | Το ύψος της σελίδας. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Ο αριθμός της σελίδας. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | Το πλάτος της σελίδας. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### Δείτε επίσης
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
