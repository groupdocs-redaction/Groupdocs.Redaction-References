---
title: "apply-Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Wendet eine Redaktion auf das Dokument an."
type: docs
url: /de/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Wendet eine Redaktion auf das Dokument an.

```python
def apply(self, redaction):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redaction | `Redaction` | Eine Instanz von `Redaction` zum Anwenden. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Beispiel

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Definieren Sie die Redaktion, um SSN‑Muster zu ersetzen
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Laden Sie das Dokument und wenden Sie die Redaktion an
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Wendet eine Menge von Redaktionen auf das Dokument an.

```python
def apply(self, redactions):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| redactions | `list[Redaction]` | Ein Array von Redaktionen zum Anwenden. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Beispiel

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

Wendet eine Redaktionsrichtlinie auf das Dokument an.

```python
def apply(self, policy):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redaktionsrichtlinie. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Beispiel

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

### Siehe auch
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
