---
title: "μέθοδος generate_preview"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας."
type: docs
url: /el/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Δημιουργεί εικόνες προεπισκόπησης συγκεκριμένων σελίδων σε δεδομένη μορφή εικόνας.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Δείτε επίσης
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
