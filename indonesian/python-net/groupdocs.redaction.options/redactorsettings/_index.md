---
title: "kelas RedactorSettings"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili pengaturan redaksi, memungkinkan menyesuaikan proses redaksi."
type: docs
url: /id/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Mewakili pengaturan redaksi, memungkinkan menyesuaikan proses redaksi.

Pelajari lebih lanjut

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

Tipe RedactorSettings menampilkan anggota-anggota berikut:

### Konstruktor
| Konstruktor | Deskripsi |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | Menginisialisasi instance baru dari kelas RedactorSettings. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Menginisialisasi instance RedactorSettings baru dengan instance ILogger yang diberikan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance IRedactionCallback yang diberikan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Menginisialisasi instance RedactorSettings baru dengan IOcrConnector yang ditentukan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Menginisialisasi instance RedactorSettings baru dengan logger dan callback yang ditentukan. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Menginisialisasi instance baru dari kelas RedactorSettings dengan instance ILogger, IRedactionCallback, dan IOcrConnector yang diberikan. |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Logger yang digunakan untuk mencatat peristiwa dan kesalahan. Harus berupa instance dari kelas yang mengimplementasikan [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/). |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | Instance konektor OCR yang mengimplementasikan [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/). |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Callback redaksi yang digunakan untuk mengevaluasi setiap deskripsi redaksi. |

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
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
