---
title: "Κλάση LoadOptions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου."
type: docs
url: /el/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Παρέχει επιλογές που θα χρησιμοποιηθούν για το άνοιγμα ενός αρχείου.

Μάθετε περισσότερα
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Ο τύπος LoadOptions εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Αρχικοποιεί ένα νέο στιγμιότυπο του LoadOptions με τον καθορισμένο κωδικό πρόσβασης. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Αρχικοποιεί ένα νέο στιγμιότυπο LoadOptions με τη συγκεκριμένη σημαία προ‑απεικόνισης. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Αρχικοποιεί ένα νέο στιγμιότυπο LoadOptions με τον καθορισμένο κωδικό πρόσβασης. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Ο κωδικός πρόσβασης για έγγραφα με προστασία κωδικού. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Η σημαία pre_rasterize υποδεικνύει αν το αρχείο πρέπει να προ‑απεικονιστεί. |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Καθορίστε τις επιλογές φόρτωσης με τον κωδικό πρόσβασης του εγγράφου
load_opt = LoadOptions("mypassword")

# Ορίστε μια διαγραφή
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Ανοίξτε το έγγραφο με προστασία κωδικού πρόσβασης
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Αποθηκεύστε το διαγραμμένο έγγραφο
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
