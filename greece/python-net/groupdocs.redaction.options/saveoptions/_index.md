---
title: "Κλάση SaveOptions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Παρέχει επιλογές για την αλλαγή του ονόματος του εξαγόμενου αρχείου και/ή τη μετατροπή του εγγράφου σε PDF βασισμένο σε εικόνα (rasterization)."
type: docs
url: /el/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Παρέχει επιλογές για την αλλαγή του ονόματος του εξαγόμενου αρχείου και/ή τη μετατροπή του εγγράφου σε PDF βασισμένο σε εικόνα (rasterization).

Μάθετε περισσότερα:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

Ο τύπος SaveOptions εκθέτει τα ακόλουθα μέλη:

### Κατασκευαστές
| Κατασκευαστής | Περιγραφή |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Αρχικοποιεί ένα νέο αντικείμενο με προεπιλεγμένες ρυθμίσεις: το rasterize_to_pdf είναι False και το add_suffix είναι False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Αρχικοποιεί ένα νέο αντικείμενο με τα δοθέντα παραμέτρους. |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | Η ιδιότητα add_suffix υποδεικνύει αν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. Η προεπιλογή είναι False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | Οι ρυθμίσεις rasterization. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | Η σημαία που υποδεικνύει αν όλες οι σελίδες του εγγράφου μετατρέπονται σε εικόνες και συνδυάζονται σε ένα ενιαίο αρχείο PDF. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Το προσαρμοσμένο επίθημα για το όνομα του αρχείου εξόδου. Εάν δεν καθοριστεί, χρησιμοποιείται η σταθερά [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/). |

### Πεδία
| Πεδίο | Περιγραφή |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Αναπαριστά την προεπιλεγμένη τιμή επιθήματος, η οποία είναι "Redacted". |

### Παράδειγμα

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Αποθηκεύστε το έγγραφο με τις προεπιλεγμένες επιλογές (rasterize to PDF και add suffix)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
Οδηγοί εργασιών που χρησιμοποιούν `SaveOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Δείτε επίσης
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
