---
title: "Kelas IRedactionCallback"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mendefinisikan metode yang diperlukan untuk menerima informasi tentang setiap perubahan redaksi dan secara opsional mencegahnya."
type: docs
url: /id/python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Mendefinisikan metode yang diperlukan untuk menerima informasi tentang setiap perubahan redaksi dan secara opsional mencegahnya.

Pelajari lebih lanjut:
- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Tipe IRedactionCallback menampilkan anggota-anggota berikut:

### Metode
| Metode | Deskripsi |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Dipicu tepat sebelum menerapkan penyensoran apa pun pada dokumen, memungkinkan pencatatan atau melarangnya. |
| [accept_redaction_redaction_description](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction_redaction_description/) |  |

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
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
