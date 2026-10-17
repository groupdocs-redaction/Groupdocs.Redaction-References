---
title: "Αποκρυπτογραφήσεις υπολογιστικών φύλλων"
linkTitle: "Spreadsheet redactions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς το Python redaction API επιτρέπει την αφαίρεση δεδομένων ευαίσθητης ή ιδιωτικής φύσης από τα μορφότυπα υπολογιστικών φύλλων XLS, XLSX, ODS και άλλα."
type: docs
url: /el/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


Το GroupDocs.Redaction επιτρέπει την αφαίρεση δεδομένων ευαίσθητης ή ιδιωτικής φύσης από τα μορφότυπα υπολογιστικών φύλλων XLS, XLSX, ODS και άλλα. Δείτε την πλήρη λίστα στο άρθρο [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Φορτώστε το υπολογιστικό φύλλο που θα υποβληθεί σε αποκρυπτογράφηση
    with Redactor("./sample.xlsx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) για να το κατεβάσετε.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
