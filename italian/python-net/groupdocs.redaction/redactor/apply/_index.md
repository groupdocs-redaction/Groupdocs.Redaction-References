---
title: "metodo apply"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Applica una redazione al documento."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Applica una redazione al documento.

```python
def apply(self, redaction):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redaction | `Redaction` | Un'istanza di `Redaction` da applicare. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Esempio

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Definisci la redazione per sostituire i pattern SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Carica il documento e applica la redazione
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Applica un insieme di redazioni al documento.

```python
def apply(self, redactions):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| redactions | `list[Redaction]` | Un array di redazioni da applicare. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Esempio

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

Applica una politica di redazione al documento.

```python
def apply(self, policy):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| policy | `RedactionPolicy` | Politica di redazione. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Esempio

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

### Vedi anche
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
