---
title: "Κλάση CreatePageStream"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια μέθοδο που επιστρέφει ένα ρεύμα για την εγγραφή δεδομένων προεπισκόπησης σελίδας."
type: docs
url: /el/python-net/groupdocs.redaction.options/createpagestream/
is_root: false
weight: 20
---


## CreatePageStream class

Αντιπροσωπεύει μια μέθοδο που επιστρέφει ένα ρεύμα για την εγγραφή δεδομένων προεπισκόπησης σελίδας.

Ο τύπος CreatePageStream εκθέτει τα παρακάτω μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/createpagestream/__init__/#object-method) |  |

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke/#page_number-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke_int32/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke/#page_number) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke_int32/) |  |

### Παράδειγμα

```python
import os
import io
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int) -> io.RawIOBase:
    page_path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(page_path, "wb")

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
