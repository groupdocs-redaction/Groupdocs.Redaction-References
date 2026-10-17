---
title: "save μέθοδος"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /el/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Αποθηκεύει το έγγραφο σε αρχείο.

```python
def save(self, save_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| save_options | `SaveOptions` | Επιλογές για προσθήκη καταλήξης ή rasterize. |

**Returns:** Path to redacted document.

### Παράδειγμα

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        redactor.apply(ex_red)

        # Αποθηκεύστε το επεξεργασμένο έγγραφο στην αρχική του μορφή με μια καταλήξη ημερομηνίας
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Αποθηκεύει το έγγραφο σε ροή, συμπεριλαμβανομένης της προσαρμοσμένης τοποθεσίας.

```python
def save(self, document, rasterization_options):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| document | `io.RawIOBase` | Στοχευμένη ροή. |
| rasterization_options | `RasterizationOptions` | Επιλογές για rasterize ή όχι και για καθορισμό σελίδων για rasterization. |

### Παράδειγμα

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # ρυθμίστε το rasterization ώστε να επεξεργάζεται μόνο την πρώτη διαφάνεια
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # το αντικείμενο BytesIO τώρα περιέχει το αποθηκευμένο έγγραφο
    data = stream.getvalue()
```

### Δείτε επίσης
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
