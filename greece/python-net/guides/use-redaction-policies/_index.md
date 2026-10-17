---
title: "Χρησιμοποιήστε πολιτικές σβησίματος"
linkTitle: "Use redaction policies"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Μάθετε πώς να το αντιμετωπίζετε. Εάν έχετε μια εταιρική πολιτική αφαίρεσης ευαίσθητων δεδομένων ως λίστα κανόνων σβησίματος, δεν χρειάζεται να τα καθορίσετε στον κώδικά σας. Μπορείτε να καθορίσετε ένα έγγραφο XML με μια λίστα προρυθμισμένων σβησίμων."
type: docs
url: /el/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Εάν έχετε μια εταιρική πολιτική αφαίρεσης ευαίσθητων δεδομένων ως λίστα κανόνων σβησίματος, δεν χρειάζεται να τα καθορίσετε στον κώδικά σας. Μπορείτε να καθορίσετε ένα έγγραφο XML με μια λίστα προρυθμισμένων σβησίμων.

Παρακάτω είναι ένα παράδειγμα αρχείου XML πολιτικής σβησίματος (η αντιστοίχηση ιδιοτήτων κώδικα είναι προφανής):

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
Μπορείτε να χρησιμοποιήσετε τη μέθοδο RedactionPolicy.save() για να δημιουργήσετε έγγραφα XML αυτής της δομής, διαμορφώνοντας τα σβησίματα κατά την εκτέλεση.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) σε αρχείο XML.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # Ορίστε το χρώμα του σβησίματος
    color = Color.from_argb(255, 220, 20, 60)

    # Διαμορφώστε τα σβησίματα
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Δημιουργήστε την πολιτική
    policy = RedactionPolicy(redactions)

    # Αποθηκεύστε την πολιτική σβησίματος σε αρχείο XML
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

Μπορείτε να έχετε όσες πολιτικές χρειάζεστε, φορτώνοντάς τες για να σβήνετε τα έγγραφά σας.

Το παρακάτω παράδειγμα φορτώνει μια πολιτική διαγραφής από ένα αρχείο XML και εφαρμόζει κάθε κανόνα που περιέχει σε ένα έγγραφο με μία ενιαία κλήση `apply`:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Φορτώστε την πολιτική διαγραφής από ένα αρχείο XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Φορτώστε το έγγραφο και εφαρμόστε ολόκληρη την πολιτική με μία κλήση
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Διατηρήστε την αρχική μορφή και προσθέστε ένα επίθημα στο όνομα εξόδου
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` είναι το αρχείο πολιτικής που χρησιμοποιείται σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) για να το κατεβάσετε.

`sample.docx` είναι το έγγραφο που διαγράφηκε σε αυτό το παράδειγμα. Κάντε κλικ [εδώ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) για να το κατεβάσετε.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
