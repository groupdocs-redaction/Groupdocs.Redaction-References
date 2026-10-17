---
title: "μέθοδος apply"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Εφαρμόζει μια επεμβαση στο έγγραφο."
type: docs
url: /el/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Εφαρμόζει μια επεμβαση στο έγγραφο.

```python
def apply(self, redaction):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redaction | `Redaction` | Μια παρουσία του `Redaction` για εφαρμογή. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Ορίστε τη διαγραφή για αντικατάσταση προτύπων SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Φορτώστε το έγγραφο και εφαρμόστε τη διαγραφή.
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Εφαρμόζει ένα σύνολο επεμβάσεων στο έγγραφο.

```python
def apply(self, redactions):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| redactions | `list[Redaction]` | Ένας πίνακας διαγραφών για εφαρμογή. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Παράδειγμα

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataSearchRedaction,
    ReplacementOptions,
)
from groupdocs.redaction.metadata import MetadataFilter

redaction_list = [
    ExactPhraseRedaction("ClientName", ReplacementOptions("[client]")),
    ExactPhraseRedaction("ClientAddress", ReplacementOptions("[address]")),
    RegexRedaction(r"\d{3}-\d{2}-\d{4}", ReplacementOptions("[ssn]")),
    RegexRedaction(r"\d{16}", ReplacementOptions("[card]")),
    DeleteAnnotationRedaction(r"(?im:(use|show|describe))"),
    EraseMetadataRedaction(MetadataFilter.Author),
    MetadataSearchRedaction("CompanyName", "--company--"),
]

with Redactor("./test.docx") as redactor:
    result = redactor.apply(redaction_list)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

## apply {#policy}

Εφαρμόζει μια πολιτική επεμβάσεων στο έγγραφο.

```python
def apply(self, policy):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| policy | `RedactionPolicy` | Πολιτική διαγραφής. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Παράδειγμα

```python
import os
from groupdocs.redaction import Redactor, RedactionPolicy, RedactionStatus
from groupdocs.redaction.options import RasterizationOptions

policy = RedactionPolicy.load("RedactionPolicy.xml")
for file_name in os.listdir(r"C:\Inbound"):
    file_path = os.path.join(r"C:\Inbound", file_name)
    with Redactor(file_path) as redactor:
        result = redactor.apply(policy)
        out_folder = (
            r"C:\Outbound\Done"
            if result.status != RedactionStatus.FAILED
            else r"C:\Outbound\Failed"
        )
        out_path = os.path.join(out_folder, file_name)
        with open(out_path, "r+b") as stream:
            redactor.save(stream, RasterizationOptions(enabled=False))
```

### Δείτε επίσης
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
