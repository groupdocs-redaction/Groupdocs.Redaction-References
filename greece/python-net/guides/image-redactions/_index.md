---
title: "Αφαίρεση εικόνων"
linkTitle: "Image redactions"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς να αφαιρέσετε δεδομένα ευαίσθητης φύσης από εικόνες διαφόρων μορφών όπως JPG, PNG, TIFF και άλλες."
type: docs
url: /el/python-net/guides/image-redactions/
is_root: false
weight: 60
---


Το GroupDocs.Redactions παρέχει ένα σύνολο λειτουργιών για την αφαίρεση δεδομένων ευαίσθητης φύσης από εικόνες διαφόρων μορφών όπως JPG, PNG, TIFF και άλλες. Δείτε την πλήρη λίστα στο άρθρο [supported document formats]().

Το GroupDocs.Redaction υποστηρίζει δύο τρόπους αφαίρεσης εικόνων, τόσο σε ξεχωριστά αρχεία εικόνας όσο και σε ενσωματωμένες εικόνες:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

Το GroupDocs.Redaction for Python μέσω .NET επιτρέπει επίσης να αλλάξετε τα μεταδεδομένα της εικόνας (π.χ. να επεξεργαστείτε τα δεδομένα EXIF μιας εικόνας ή να λειτουργήσετε ως «σβήστρα EXIF»).

## Redact image area

Για να αφαιρέσετε περιοχή εικόνας, πρέπει να χρησιμοποιήσετε την κλάση [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Ορίστε τη θέση πάνω‑αριστερά της περιοχής που θα αφαιρεθεί
    sample_point = Point(385, 485)
    # Ορίστε το μέγεθος της περιοχής που πρέπει να αφαιρεθεί
    sample_size = Size(1793, 2069)
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.jpg") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Από προεπιλογή, το σήμανε έγγραφο αποθηκεύεται σε μορφή PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) για να το κατεβάσετε.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Εάν η αφαίρεση δεν μπορεί να εφαρμοστεί σε αυτόν τον τύπο αρχείων, π.χ. έγγραφο MS Word χωρίς ενσωματωμένες εικόνες, το [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) θα είναι [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

Το παρακάτω παράδειγμα δείχνει πώς να επεξεργαστείτε τα δεδομένα exif (να τα διαγράψετε) από μια φωτογραφία ή οποιαδήποτε άλλη εικόνα:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Καθορίστε τις επιλογές αφαίρεσης για να αφαιρέσετε όλα τα μεταδεδομένα της εικόνας (π.χ. EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Φορτώστε την εικόνα που θα αφαιρεθεί
    with Redactor("./sample.jpg") as redactor:
        # Εφαρμόστε τη διαγραφή
        result = redactor.apply(er_opt)

        # Αποθηκεύστε την επεξεργασμένη εικόνα δίπλα στο αρχικό αρχείο
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) για να το κατεβάσετε.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Εάν η αφαίρεση δεν μπορεί να εφαρμοστεί σε αυτόν τον τύπο αρχείων, π.χ. εικόνα BMP, το [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) θα είναι [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Μπορείτε να αφαιρέσετε περιοχές εικόνας σε όλα τα είδη ενσωματωμένων εικόνων μέσα σε ένα έγγραφο.

Το παρακάτω παράδειγμα δείχνει πώς να αφαιρέσετε όλες τις ενσωματωμένες εικόνες μέσα σε ένα έγγραφο Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Ορίστε τη θέση πάνω‑αριστερά της περιοχής που θα αφαιρεθεί
    sample_point = Point(516, 311)
    # Ορίστε το μέγεθος της περιοχής που πρέπει να αφαιρεθεί
    sample_size = Size(170, 35)
    # Ορίστε το χρώμα του πλαισίου διαγραφής
    color = Color.from_argb(255, 220, 20, 60)

    # Καθορίστε τις επιλογές αποκρυπτογράφησης
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Φορτώστε το έγγραφο που θα υποβληθεί σε σβήσιμο
    with Redactor("./sample.docx") as redactor:
        # Εφαρμόστε την αφαίρεση σε όλες τις ενσωματωμένες εικόνες
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Από προεπιλογή, το σήμανε έγγραφο αποθηκεύεται σε μορφή PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` είναι το δείγμα αρχείου που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Εάν η αφαίρεση δεν μπορεί να εφαρμοστεί σε αυτόν τον τύπο αρχείων, π.χ. ένα έγγραφο λογιστικού φύλλου, το [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) θα είναι [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Μπορείτε να αφαιρέσετε καρέ από μια εικόνα πολλαπλών καρέ με δεδομένη προέλευση και αριθμό καρέ. Για περισσότερες πληροφορίες, δείτε το άρθρο [remove page redactions]().

Ορισμένες μορφές εικόνας, όπως τα έγγραφα DjVu, απαιτούν [pre-rasterization]() και περαιτέρω αποθήκευση σε μορφή PDF.
