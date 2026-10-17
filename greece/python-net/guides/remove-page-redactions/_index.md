---
title: "Κατάργηση επεξεργασιών σελίδων"
linkTitle: "Remove page redactions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς να αφαιρέσετε σελίδες με ευαίσθητα δεδομένα από τα PDF, τις παρουσιάσεις και τα φύλλα εργασίας σας."
type: docs
url: /el/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction επιτρέπει την εύκολη αφαίρεση σελίδων από έγγραφα PDF, διαφάνειες από παρουσιάσεις και φύλλα εργασίας από έγγραφα λογιστικών φύλλων.

Με το GroupDocs.Redaction API μπορείτε να αφαιρέσετε σελίδες καθορίζοντας το εύρος σελίδων με βάση τη σχετική θέση της (την αρχή ή το τέλος), τον μηδενικό δείκτη και τον αριθμό των σελίδων προς αφαίρεση. Προς το παρόν οι υποστηριζόμενες μορφές είναι: PDF, παρουσιάσεις (Microsoft PowerPoint, OpenOffice Presentations), έγγραφα επεξεργασίας κειμένου (Microsoft Word, OpenOffice Texts, Rich Text Files), λογιστικά φύλλα (Microsoft Excel, OpenOffice Spreadsheets, κ.λπ.) και εικόνες πολλαπλών πλαισίων.

## Remove page range

Στο παρακάτω παράδειγμα, αφαιρούμε τη 2η, 3η και 4η σελίδα από το έγγραφο, εφόσον το έγγραφο έχει αρκετές σελίδες:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./multipage_sample.pdf") as redactor:
        # Λήψη πληροφοριών εγγράφου
        doc_info = redactor.get_document_info()

        # Απαιτείται τουλάχιστον 4 σελίδες
        if doc_info.page_count > 3:
            # Αφαίρεση 3 σελίδων ξεκινώντας από τη 2η (μηδενικός δείκτης 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Εφαρμόστε τη διαγραφή
            result = redactor.apply(rem_opt)

            # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) για να το κατεβάσετε.

## Remove last page

Σε ορισμένες περιπτώσεις μπορεί να χρειαστεί να διαγράψετε την τελευταία σελίδα ή έναν αριθμό σελίδων, ανεξάρτητα από το πόσες σελίδες υπάρχουν.

Το παρακάτω παράδειγμα δείχνει πώς να αφαιρέσετε την τελευταία σελίδα από ένα έγγραφο:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Αφαίρεση 1 σελίδας, μετρώντας από το τέλος του εγγράφου
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./multipage_sample.pdf") as redactor:
        # Λήψη πληροφοριών εγγράφου
        doc_info = redactor.get_document_info()

        # Απαιτείται τουλάχιστον 2 σελίδες ώστε το έγγραφο να μην μείνει κενό
        if doc_info.page_count > 1:
            # Εφαρμόστε τη διαγραφή
            result = redactor.apply(rem_opt)

            # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) για να το κατεβάσετε.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Σε περίπτωση εικόνας πολλαπλών πλαισίων μπορεί να χρειαστεί να διαγράψετε έναν αριθμό πλαισίων (θεωρούνται ως "σελίδες").

Το παρακάτω παράδειγμα δείχνει πώς να αφαιρέσετε 3 πλαίσια από μια κινούμενη εικόνα GIF:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Αφαίρεση πλαισίων ξεκινώντας από το 3ο (μηδενικός δείκτης 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Φορτώστε την εικόνα πολλαπλών πλαισίων που θα υποβληθεί σε επεξεργασία
    with Redactor("./sample.gif") as redactor:
        # Λήψη πληροφοριών εγγράφου
        doc_info = redactor.get_document_info()

        # Απαιτείται τουλάχιστον 7 πλαίσια
        if doc_info.page_count >= 7:
            # Εφαρμόστε τη διαγραφή
            result = redactor.apply(rem_opt)

            # Αποθηκεύστε την επεξεργασμένη εικόνα δίπλα στο αρχικό αρχείο
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) για να το κατεβάσετε.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
