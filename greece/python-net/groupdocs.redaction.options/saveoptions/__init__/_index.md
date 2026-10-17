---
title: "Κατασκευαστής __init__"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αρχικοποιεί ένα νέο αντικείμενο με προεπιλεγμένες ρυθμίσεις: rasterizetopdf είναι False και addsuffix είναι False."
type: docs
url: /el/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Αρχικοποιεί ένα νέο αντικείμενο με προεπιλεγμένες ρυθμίσεις: το rasterize_to_pdf είναι False και το add_suffix είναι False.

```python
def __init__(self):
    ...
```

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Αρχικοποιεί ένα νέο αντικείμενο με τα δοθέντα παραμέτρους.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, εάν όλες οι σελίδες στο έγγραφο πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
| suffix | `str` | Αυτό το κείμενο θα προστεθεί στο τέλος του ονόματος αρχείου· εάν δεν είναι κενό, επίσης ορίζει το `add_suffix` σε True. |

### Παράδειγμα

```python
from groupdocs.redaction.options import SaveOptions

# Δημιουργήστε επιλογές αποθήκευσης με προεπιλεγμένες ρυθμίσεις
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Δείτε επίσης
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
