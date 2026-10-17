---
title: "Διαγραφές σχολίων"
linkTitle: "Annotation redactions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει την υλοποίηση της διαγραφής σχολίων για έγγραφα διαφορετικών μορφών όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα."
type: docs
url: /el/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Με το API του GroupDocs.Redaction μπορείτε να εφαρμόσετε διαγραφές σχολίων για έγγραφα διαφορετικών μορφών όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα. Δείτε την πλήρη λίστα στο άρθρο [υποστηριζόμενες μορφές εγγράφων]().

Το GroupDocs.Redactions παρέχει ένα ευέλικτο API που επιτρέπει την αφαίρεση ευαίσθητων δεδομένων από το κείμενο των σχολίων, ή την πλήρη αφαίρεση σχολίων με κανονική έκφραση.

## Remove annotations (comments etc)

Μπορείτε να χρησιμοποιήσετε το GroupDocs.Redaction για να αφαιρέσετε όλα ή συγκεκριμένα σχόλια και άλλες σημειώσεις από το έγγραφο. Για παράδειγμα, μπορούμε να αφαιρέσουμε όλα τα σχόλια από το έγγραφο που περιέχουν κείμενα όπως "use", "show" ή "describe" στο σώμα του:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Καθορίστε τις επιλογές διαγραφής για να διαγράψετε σημειώσεις που ταιριάζουν με το μοτίβο
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./annotated.xlsx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(a_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) για να το κατεβάσετε.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Μπορείτε να χρησιμοποιήσετε τον κατασκευαστή χωρίς ορίσματα για να αφαιρέσετε όλες τις σημειώσεις μέσα στο έγγραφο.

## Redact annotations

Αντί να αφαιρέσετε όλες ή συγκεκριμένες σημειώσεις, μπορείτε να αφαιρέσετε ευαίσθητα δεδομένα από το κείμενο της σημείωσης. Για παράδειγμα, μπορούμε να αφαιρέσουμε όλες τις αναφορές στο "John" στο συγκεκριμένο έγγραφο, π.χ.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Καθορίστε τις επιλογές σβησίματος: πρότυπο αναζήτησης και συμβολοσειρά αντικατάστασης
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./annotated.xlsx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(a_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) για να το κατεβάσετε.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
