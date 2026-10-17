---
title: "Γειά σου, Κόσμε!"
linkTitle: "Hello, World!"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Ξεκινήστε γρήγορα με το GroupDocs.Redaction for Python via .NET δημιουργώντας και εκτελώντας ένα απλό παράδειγμα."
type: docs
url: /el/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Ένα παράδειγμα "Γειά σου, Κόσμε!" είναι συχνά το πρώτο βήμα όταν εξερευνάτε το GroupDocs.Redaction for Python via .NET. Λειτουργεί ως απλό τεστ για να επιβεβαιώσετε ότι το περιβάλλον ανάπτυξής σας είναι σωστά ρυθμισμένο και ότι η βιβλιοθήκη λειτουργεί όπως αναμένεται.

## Overview
Το GroupDocs.Redaction for Python via .NET σας επιτρέπει να αναζητάτε, να διαγράφετε και να αφαιρείτε ευαίσθητες πληροφορίες από διάφορες μορφές εγγράφων. Ένα ευρύ φάσμα [υποστηριζόμενων μορφών](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) το καθιστά ευέλικτο για διαφορετικές περιπτώσεις χρήσης.

## How to redact a document
Τα παρακάτω βήματα δείχνουν πώς να διαγράψετε ευαίσθητες πληροφορίες από ένα έγγραφο χρησιμοποιώντας το GroupDocs.Redaction for Python via .NET:

1. Εισάγετε τις κλάσεις `groupdocs.redaction` που χρειάζεστε.
2. Περιγράψτε τη διαγραφή (εδώ, μια ακριβής φράση που θα αντικατασταθεί με ένα χρωματιστό πλαίσιο).
3. Δημιουργήστε ένα αντικείμενο [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) με τη διαδρομή προς το δείγμα εγγράφου.
4. Εφαρμόστε τη διαγραφή.
5. Αποθηκεύστε το αποτέλεσμα.

## Complete example
Το παρακάτω παράδειγμα αντικαθιστά κάθε εμφάνιση της φράσης "John Doe" με ένα ημιδιαφανές κόκκινο πλαίσιο και αποθηκεύει το διαγραμμένο έγγραφο:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Σχεδιάστε ένα ημιδιαφανές κόκκινο πλαίσιο πάνω σε κάθε εμφάνιση του "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Φορτώστε το έγγραφο, εφαρμόστε τη διαγραφή και αποθηκεύστε το αποτέλεσμα
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Αυτό το παράδειγμα μετατρέπει το αποτέλεσμα σε PDF με όνομα `sample_redacted.pdf`, ώστε το διαγραμμένο περιεχόμενο να μην μπορεί να ανακτηθεί (`save()` μετατρέπει σε PDF εξ ορισμού· η επιλογή `redacted_file_suffix` ελέγχει μόνο το όνομα εξόδου). Για να διατηρήσετε την αρχική μορφή, ορίστε `rasterize_to_pdf = False`.

## Additional resources
Αυτή η παρουσίαση αναφέρει τα [δείγματα κώδικα](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) του GroupDocs.Redaction for Python via .NET.
