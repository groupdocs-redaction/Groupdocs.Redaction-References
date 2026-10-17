---
title: "método apply"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Aplica una redacción al documento."
type: docs
url: /es/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Aplica una redacción al documento.

```python
def apply(self, redaction):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redaction | `Redaction` | Una instancia de `Redaction` para aplicar. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Ejemplo

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Defina la redacción para reemplazar los patrones de SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Cargue el documento y aplique la redacción
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Aplica un conjunto de redacciones al documento.

```python
def apply(self, redactions):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| redactions | `list[Redaction]` | Una matriz de redacciones para aplicar. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Ejemplo

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

Aplica una política de redacción al documento.

```python
def apply(self, policy):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| policy | `RedactionPolicy` | Política de redacción. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Ejemplo

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

### Ver también
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
