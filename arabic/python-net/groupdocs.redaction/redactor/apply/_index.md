---
title: "طريقة apply"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يطبق حذفًا على المستند."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/apply/
is_root: false
weight: 1010
---


## apply {#redaction}

يطبق حذفًا على المستند.

```python
def apply(self, redaction):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redaction | `Redaction` | كائن من `Redaction` لتطبيقه. |

**Returns:** RedactorChangeLog: Indicates success or failure and includes an error message when the operation fails.

### مثال

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions

def apply_redaction():
    # حدد عملية الحذف لاستبدال أنماط رقم الضمان الاجتماعي
    ssn_redaction = RegexRedaction(r"\b\d{3}-\d{2}-\d{4}\b", ReplacementOptions("[ssn]"))

    # حمّل المستند وطبق الحذف.
    with Redactor("./test.docx") as redactor:
        result = redactor.apply(ssn_redaction)

        if result.status != RedactionStatus.FAILED:
            redactor.save()
```

## apply {#redactions}

يطبق مجموعة من عمليات الحذف على المستند.

```python
def apply(self, redactions):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| redactions | `list[Redaction]` | مصفوفة من عمليات الحذف للتطبيق. |

**Returns:** RedactorChangeLog: Indicates success or failure and contains an error message if applicable.

### مثال

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

يطبق سياسة حذف على المستند.

```python
def apply(self, policy):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| policy | `RedactionPolicy` | سياسة الحذف. |

**Returns:** `RedactorChangeLog`: Indicates success or failure and contains an error message if the operation failed.

### مثال

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

### انظر أيضًا
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
