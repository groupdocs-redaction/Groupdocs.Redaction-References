---
title: "metode accept_redaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Dipicu tepat sebelum menerapkan penyensoran apa pun pada dokumen, memungkinkan pencatatan atau melarangnya."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/
is_root: false
weight: 1010
---


## accept_redaction {#description}

Dipicu tepat sebelum menerapkan penyensoran apa pun pada dokumen, memungkinkan pencatatan atau melarangnya.

```python
def accept_redaction(self, description):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| description | `RedactionDescription` | Berisi informasi tentang tipe kecocokan tertentu, kriteria, teks, dan posisi. |

**Returns:** bool: True to accept the redaction, False to decline it.

### Contoh

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction.options import LoadOptions, RedactorSettings

def accept(description):
    # description.original_text, .redaction_type, .action_type
    return "keep-me" not in (description.original_text or "")

with Redactor("document.docx", LoadOptions(), RedactorSettings(callback=accept)) as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### Lihat Juga
* class [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/)
