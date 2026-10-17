---
title: "metode apply"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menerapkan redaksi pada dokumen."
type: docs
url: /id/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Menerapkan redaksi pada dokumen.

```python
def apply(self, redaction):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redaction | `Redaction` | Sebuah instance dari `Redaction` untuk diterapkan. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Contoh

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Tentukan redaksi untuk mengganti pola SSN
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Muat dokumen dan terapkan redaksi
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Menerapkan sekumpulan redaksi pada dokumen.

```python
def apply(self, redactions):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redactions | `list[Redaction]` | Sebuah array redaksi untuk diterapkan. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Contoh

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

Menerapkan kebijakan redaksi pada dokumen.

```python
def apply(self, policy):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| policy | `RedactionPolicy` | Kebijakan redaksi. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Contoh

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

### Lihat Juga
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
