---
title: "méthode apply"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Applique une rédaction au document."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Applique une rédaction au document.

```python
def apply(self, redaction):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redaction | `Redaction` | Une instance de `Redaction` à appliquer. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Exemple

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Définissez la redaction pour remplacer les modèles de SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Chargez le document et appliquez la redaction
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Applique un ensemble de rédactions au document.

```python
def apply(self, redactions):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| redactions | `list[Redaction]` | Un tableau de redactions à appliquer. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Exemple

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

Applique une politique de rédaction au document.

```python
def apply(self, policy):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| policy | `RedactionPolicy` | Politique de redaction. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Exemple

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

### Voir aussi
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
