---
title: apply method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Applies a redaction to the document."
type: docs
url: /python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

Applies a redaction to the document.

```python
def apply(self, redaction):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redaction | `Redaction` | An instance of `Redaction` to apply. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### Example

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # Define the redaction to replace SSN patterns
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # Load the document and apply the redaction
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

Applies a set of redactions to the document.

```python
def apply(self, redactions):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| redactions | `list[Redaction]` | An array of redactions to apply. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### Example

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

Applies a redaction policy to the document.

```python
def apply(self, policy):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| policy | `RedactionPolicy` | Redaction policy. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### Example

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

### See Also
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
