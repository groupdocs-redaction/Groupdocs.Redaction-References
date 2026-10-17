---
title: "Αποκρυπτογραφήσεις μεταδεδομένων"
linkTitle: "Metadata redactions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς το Python redaction API σας επιτρέπει να αντικαταστήσετε ή να αφαιρέσετε μεταδεδομένα χρησιμοποιώντας φίλτρα ή αναζήτηση με κανονική έκφραση."
type: docs
url: /el/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Με το GroupDocs.Redaction API μπορείτε να εφαρμόσετε αποκρυπτογραφήσεις μεταδεδομένων για έγγραφα διαφορετικών μορφών όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα. Δείτε την πλήρη λίστα στο άρθρο [supported document formats]().

Το GroupDocs.Redactions παρέχει ένα ευέλικτο API που επιτρέπει την αντικατάσταση ή αφαίρεση μεταδεδομένων χρησιμοποιώντας φίλτρα ή αναζήτηση με κανονική έκφραση.

## Filter metadata

Η βασική λειτουργικότητα για όλες τις αποκρυπτογραφήσεις, που προέρχεται από τη βασική κλάση [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/), είναι *metadata filtering* και είναι υποχρεωτική για τις αποκρυπτογραφήσεις μεταδεδομένων. Χρησιμοποιεί την σηματοδοτημένη απαρίθμηση [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), η οποία περιέχει στοιχεία για τις πιο συχνές καταχωρήσεις μεταδεδομένων. Μπορείτε να ορίσετε το φίλτρο σε *All*, ή σε οποιονδήποτε συνδυασμό μεταδεδομένων. Για παράδειγμα, το παρακάτω δείγμα ορίζει το φίλτρο σε *Author*, *Manager* και *NameOfApplication* - για κειμενική αποκρυπτογράφηση ή καθαρισμό τους:

```python
# αποκρυπτογράφηση που προέρχεται από το MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Παρακάτω είναι ο πίνακας με την πλήρη λίστα των στοιχείων του [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Φίλτρο | Αριθμητική τιμή | Περιγραφή |
| --- | --- | --- |
| *None* | 0 | Κενή ρύθμιση φίλτρου, δεν ταιριάζει με κανένα στοιχείο μεταδεδομένων |
| *Author* | 1 | Συγγραφέας του εγγράφου |
| *Κατηγορία* | 2 | Κατηγορία του εγγράφου |
| *Σχόλια* | 4 | Σχόλιο εγγράφου |
| *Εταιρεία* | 8 | Εταιρεία του Συγγραφέα |
| *ContentStatus* | 16 | Κατάσταση περιεχομένου |
| *CreatedTime* | 32 | Ώρα δημιουργίας |
| *HyperlinkBase* | 64 | Βάση υπερσύνδεσμου |
| *LastPrinted* | 128 | Ημερομηνία και ώρα τελευταίας εκτύπωσης |
| *LastSavedBy* | 256 | Τελευταία αποθήκευση από τον χρήστη |
| *LastSavedTime* | 1024 | Ημερομηνία και ώρα τελευταίας αποθήκευσης |
| *NameOfApplication* | 2048 | Όνομα της εφαρμογής όπου δημιουργήθηκε το έγγραφο |
| *Manager* | 4096 | Όνομα του διευθυντή του συγγραφέα |
| *RevisionNumber* | 8192 | Αριθμός αναθεώρησης |
| *Subject* | 16384 | Θέμα του εγγράφου |
| *Template* | 32768 | Όνομα προτύπου εγγράφου |
| *Title* | 65536 | Τίτλος εγγράφου |
| *TotalEditingTime* | 131072 | Συνολικός χρόνος επεξεργασίας |
| *Έκδοση* | 262144 | Έκδοση εγγράφου |
| *Περιγραφή* | 524288 | Περιγραφή εγγράφου |
| *Λέξεις-κλειδιά* | 1048576 | Λέξεις-κλειδιά εγγράφου |
| *ContentType* | 2097152 | Τύπος περιεχομένου |
| *Όλα* | 2147483647 | Όλοι οι τύποι των στοιχείων μεταδεδομένων |

## Clean metadata

Μπορείτε να αντικαταστήσετε όλα ή συγκεκριμένα μεταδεδομένα στο έγγραφο με κενές (κενές ή ελάχιστες) τιμές χρησιμοποιώντας την κλάση [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) . Το παρακάτω παράδειγμα αφαιρεί όλες τις ιδιότητες του εγγράφου:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Καθορίστε τις επιλογές σβησίματος για να αφαιρέσετε όλα τα μεταδεδομένα
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(met_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Μπορείτε να καθορίσετε [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) ή να χρησιμοποιήσετε τον προεπιλεγμένο κατασκευαστή για να αφαιρέσετε όλα τα μεταδεδομένα μέσα στο συγκεκριμένο έγγραφο, Custom - για να διαγράψετε όλες τις προσαρμοσμένες καταχωρήσεις μεταδεδομένων.

## Redact metadata

Μπορείτε να χρησιμοποιήσετε [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) για να αφαιρέσετε ευαίσθητα δεδομένα από τα μεταδεδομένα του εγγράφου χρησιμοποιώντας κανονικές εκφράσεις. Για παράδειγμα, μπορούμε να αφαιρέσουμε οποιαδήποτε αναφορά στο "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Καθορίστε τις επιλογές σβησίματος: πρότυπο αναζήτησης και συμβολοσειρά αντικατάστασης
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(met_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Το πρώτο όρισμα είναι κανονική έκφραση, το δεύτερο είναι μια συμβολοσειρά αντικατάστασης. Μπορείτε επίσης να ορίσετε το πεδίο εφαρμογής του σβησίματος ορίζοντας φίλτρο, π.χ. σε [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - θα αφήσει τα ταιριάσματα των κανονικών εκφράσεων ακατάργητα σε όλα τα στοιχεία μεταδεδομένων, εκτός από την ιδιότητα "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Καθορίστε τις επιλογές σβησίματος: πρότυπο αναζήτησης και συμβολοσειρά αντικατάστασης
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Περιορίστε το πεδίο σβησίματος μόνο στο στοιχείο μεταδεδομένων Company
    met_red.filter = MetadataFilters.COMPANY

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(met_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Όλες οι σβησίμες μεταδεδομένων εφαρμόζονται σε κάθε στοιχείο μεταδεδομένων ξεχωριστά, και ακόμη και αν η σβήση ενός στοιχείου αποτύχει, τα υπόλοιπα στοιχεία μεταδεδομένων θα ενημερωθούν. Μπορείτε να βρείτε μια λίστα με αποτυχημένα, παραλειπόμενα (απορριφθέντα) στοιχεία μεταδεδομένων και τους λόγους για αυτό στην ιδιότητα [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) του [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
