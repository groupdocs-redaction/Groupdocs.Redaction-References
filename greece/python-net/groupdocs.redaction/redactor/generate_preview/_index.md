---
title: "μέθοδος generate_preview"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας."
type: docs
url: /el/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας.

Η προεπισκόπηση παράγεται σύμφωνα με τις ρυθμίσεις που ορίζονται στο `preview_options`, οι οποίες περιλαμβάνουν μορφή εικόνας, διαστάσεις, εύρος σελίδων και κλήσεις επιστροφής για δημιουργία και απελευθέρωση ροών σελίδων.

```python
def generate_preview(self, preview_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Ιδιότητες εικόνας και ρυθμίσεις εύρους σελίδων. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Επιστρέφει μια εγγράψιμη ροή αρχείου για την εικόνα προεπισκόπησης της δεδομένης σελίδας.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Καλείται μετά τη γραφή της εικόνας προεπισκόπησης.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Δείτε επίσης
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
