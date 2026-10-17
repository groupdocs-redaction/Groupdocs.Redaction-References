---
title: "apply‑methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Past een redactie toe op het document."
type: docs
url: /nl/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Past een redactie toe op het document.

```python
def apply(self, redaction):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redaction | `Redaction` | Een instantie van `Redaction` om toe te passen. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Voorbeeld

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Definieer de redactie om SSN‑patronen te vervangen.
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Laad het document en pas de redactie toe.
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Past een reeks redacties toe op het document.

```python
def apply(self, redactions):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| redactions | `list[Redaction]` | Een array van redacties om toe te passen. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Voorbeeld

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

Past een redactiebeleid toe op het document.

```python
def apply(self, policy):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redactiebeleid. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Voorbeeld

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

### Zie ook
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
