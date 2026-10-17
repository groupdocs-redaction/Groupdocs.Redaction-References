---
title: "Επεξεργασία κειμένου"
linkTitle: "Text redaction"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο εξηγεί πώς το Python redaction API σας επιτρέπει να επεξεργάζεστε εύκολα δεδομένα ευαίσθητης ή ιδιωτικής φύσης από τα έγγραφά σας. Μπορείτε να εφαρμόσετε επεξεργασία κειμένου χρησιμοποιώντας ακριβή φράση ή κανονική έκφραση για έγγραφα διαφορετικών μορφών όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα."
type: docs
url: /el/python-net/guides/text-redactions/
is_root: false
weight: 50
---


Το GroupDocs.Redaction επιτρέπει την εύκολη επεξεργασία δεδομένων ευαίσθητης ή ιδιωτικής φύσης από τα έγγραφά σας. Η πιο δημοφιλής περίπτωση επεξεργασίας είναι η αφαίρεση κειμένου από ένα έγγραφο.

Με το GroupDocs.Redaction API μπορείτε να εφαρμόσετε επεξεργασία κειμένου χρησιμοποιώντας ακριβή φράση ή [regular expression](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) για έγγραφα διαφορετικών μορφών όπως PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX και άλλα. Δείτε την πλήρη λίστα στο άρθρο [supported document formats]().

## Use exact phrase redaction

Στο παρακάτω παράδειγμα, εφαρμόζουμε επεξεργασία κειμένου, αντικαθιστώντας την προσωπική ακριβή φράση "John Doe" με "\[personal\]" (ή οποιονδήποτε κωδικό εξαίρεσης):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Από προεπιλογή, η αναζήτηση για ακριβή φράση δεν διακρίνει πεζά-κεφαλαία. Για μια διαγραφή με διάκριση πεζών-κεφαλαίων, υπάρχει μια παράμετρος κατασκευής και η αντίστοιχη δημόσια ιδιότητα:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Ενεργοποίηση ταίριασματος με διάκριση πεζών-κεφαλαίων
    case_sensitive = True

    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Εάν χρειάζεστε ένα χρωματικό πλαίσιο πάνω από το κείμενο που έχει διαγραφεί, μπορείτε να χρησιμοποιήσετε χρώμα αντί για συμβολοσειρά αντικατάστασης. Η διαγραφή θα διαγράψει το ταιριασμένο κείμενο και θα τοποθετήσει ένα ορθογώνιο του καθορισμένου χρώματος στη θέση του διαγραμμένου κειμένου:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Μπορεί να χρειαστεί να εφαρμόσετε διαγραφή σε έγγραφο από δεξιά προς αριστερά, όπως τα Αραβικά ή τα Εβραϊκά. Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε το ExactPhraseRedaction σε ένα Αραβικό PDF έγγραφο:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Καθορίστε τις επιλογές διαγραφής με μια αραβική φράση
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./arabic.pdf") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(ex_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) για να το κατεβάσετε.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Πίσω από τη σκηνή, η διαγραφή "ακριβής φράση" λειτουργεί μέσω κανονικών εκφράσεων, που είναι η βασική προσέγγιση για τη διαγραφή. Στο παρακάτω παράδειγμα, διαγράφουμε οποιοδήποτε κείμενο που ταιριάζει με "2 ψηφία, κενό ή τίποτα, 2 ψηφία, ξανά κενό και 6 ψηφία" χρησιμοποιώντας ένα μπλε χρωματικό πλαίσιο:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(reg_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` είναι το αρχείο δείγμα που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Εάν χρειάζεστε να διαγράψετε ολόκληρη παράγραφο, ίσως χρειαστεί επίσης να χρησιμοποιήσετε το RegexRedaction. Το παρακάτω παράδειγμα δείχνει πώς να διαγράψετε ολόκληρη την παράγραφο σε ένα PDF έγγραφο:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Καθορίστε τις επιλογές διαγραφής που ταιριάζουν με ολόκληρη παράγραφο
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.pdf") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(reg_red)

        # Αποθηκεύστε το αποκρυπτογραφημένο έγγραφο δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) για να το κατεβάσετε.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
