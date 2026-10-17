---
title: "apply मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ पर एक रेडैक्शन लागू करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

दस्तावेज़ पर एक रेडैक्शन लागू करता है।

```python
def apply(self, redaction):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redaction | `Redaction` | `Redaction` का एक इंस्टेंस लागू करने के लिए। |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### उदाहरण

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # SSN पैटर्न को बदलने के लिए रेडैक्शन परिभाषित करें
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # दस्तावेज़ लोड करें और रेडैक्शन लागू करें
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

दस्तावेज़ पर रेडैक्शन का एक सेट लागू करता है।

```python
def apply(self, redactions):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redactions | `list[Redaction]` | लागू करने के लिए रेडैक्शनों की एक एरे। |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### उदाहरण

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

दस्तावेज़ पर एक रेडैक्शन नीति लागू करता है।

```python
def apply(self, policy):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| policy | `RedactionPolicy` | रेडैक्शन नीति। |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### उदाहरण

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

### संबंधित देखें
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
