---
title: "Βασικές αρχές διαγραφής"
linkTitle: "Redaction basics"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς οι προγραμματιστές Python μπορούν να εφαρμόσουν διαγραφή μεταδεδομένων, εικόνας, σχολίων και κειμένου στα έγγραφά τους. Υποστηρίζεται ευρύ φάσμα μορφών εγγράφων, όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα."
type: docs
url: /el/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


Το GroupDocs.Redaction υποστηρίζει ένα αποτελεσματικό σύνολο λειτουργιών διαγραφής εγγράφων. Επιτρέπει την εφαρμογή διαγραφών για [text](), [metadata](), [annotations](), [images]().

Υποστηρίζεται ευρύ φάσμα μορφών εγγράφων, όπως: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα. Δείτε την πλήρη λίστα των υποστηριζόμενων μορφών στο άρθρο [supported document formats]().

## Redaction types

Το GroupDocs.Redaction περιλαμβάνει τους παρακάτω τύπους διαγραφής:

| Τύπος | Περιγραφή | Κλάσεις |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Η εφαρμογή σήμανσης σε ένα έγγραφο γίνεται μέσω της μεθόδου [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . Ως αποτέλεσμα, λαμβάνετε το αντικείμενο [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) , το οποίο περιέχει μια καταχώρηση καταγραφής για κάθε εφαρμοσμένη σήμανση. Η καταχώρηση περιέχει αναφορά στο αντικείμενο [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) συμπεριλαμβανομένων των επιλογών του, της κατάστασης της λειτουργίας (δείτε παρακάτω) και των περιγραφών κειμένου όταν είναι εφαρμόσιμες. Εάν τουλάχιστον μία σήμανση απέτυχε, θα δείτε το [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Όλες οι πιθανές καταστάσεις της απαρίθμησης [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) εμφανίζονται σε αυτόν τον πίνακα:

| Κατάσταση | Περιγραφή | Πιθανές αιτίες |
| --- | --- | --- |
| *Applied* | Η σήμανση εφαρμόστηκε πλήρως και επιτυχώς | Όλες οι λειτουργίες εντός της διαδικασίας σήμανσης εφαρμόστηκαν επιτυχώς |
| *PartiallyApplied* | Η σήμανση εφαρμόστηκε μόνο σε μέρος των αντιστοιχίσεων της | 1) Οι περιορισμοί δοκιμής για αντικαταστάσεις υπερέβησαν2) Τουλάχιστον μια αλλαγή απορρίφθηκε από τον χρήστη |
| *Skipped* | Η σήμανση παραλήφθηκε (δεν εφαρμόστηκε) | 1) Οι περιορισμοί δοκιμής για σήμανση υπερέβησαν2) Η σήμανση δεν μπορεί να εφαρμοστεί σε αυτόν τον τύπο εγγράφου3) Όλες οι αντικαταστάσεις απορρίφθηκαν από τον χρήστη και δεν έγιναν αλλαγές |
| *Failed* | Η σήμανση απέτυχε με εξαίρεση | Παρουσιάστηκε εξαίρεση στη διαδικασία σήμανσης |

Για λεπτομερείς πληροφορίες πρέπει να επαναλάβετε τις καταχωρήσεις του καταγραφικού σήμανσης στο [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) και να ελέγξετε την ιδιότητα [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) των στοιχείων με κατάσταση διαφορετική από *Applied*:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Από προεπιλογή, το σήμανε έγγραφο αποθηκεύεται σε μορφή PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Εξαγωγή όλων των αποτυχημένων ή παραλειπόμενων σήμανσεων
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Μπορείτε να εφαρμόσετε όσες σήμανσεις χρειάζεστε σε μία κλήση στη μέθοδο [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , καθώς η υπερφόρτωση της δέχεται έναν πίνακα σήμανσεων και πολιτική σήμανσης. Σε αυτήν την περίπτωση, οι σήμανσεις θα εφαρμοστούν με την ίδια σειρά με την οποία εμφανίζονται στον πίνακα. Ως εναλλακτική λύση για τον καθορισμό συνόλων σήμανσης στον κώδικά σας, μπορείτε να δημιουργήσετε ένα αρχείο XML με πολιτική σήμανσης, όπως περιγράφεται [εδώ]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Παρέχετε μια λίστα σήμανσεων για εφαρμογή με τη σωστή σειρά
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη λίστα των διαγραφών
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Από προεπιλογή, το σήμανε έγγραφο αποθηκεύεται σε μορφή PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Εξαγωγή όλων των αποτυχημένων ή παραλειπόμενων σήμανσεων
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
