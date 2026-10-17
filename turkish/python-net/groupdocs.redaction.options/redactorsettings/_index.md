---
title: "RedactorSettings sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Redaksiyon sürecini özelleştirmeye izin veren redaksiyon ayarlarını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.options/redactorsettings/
is_root: false
weight: 90
---


## RedactorSettings class

Redaksiyon sürecini özelleştirmeye izin veren redaksiyon ayarlarını temsil eder.

Daha fazla bilgi edinin

- More details about implementing ILogger interface: [Use advanced logging](https://docs.groupdocs.com/redaction/net/use-advanced-logging/)
- More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

RedactorSettings türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/) | RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger) | Verilen bir ILogger örneği ile yeni bir RedactorSettings örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#callback) | Verilen bir IRedactionCallback örneği ile RedactorSettings sınıfının yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#ocr_connector) | Belirtilen IOcrConnector ile yeni bir RedactorSettings örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback) | Belirtilen logger ve geri çağırma ile yeni bir RedactorSettings örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/redactorsettings/__init__/#logger-callback-ocr_connector) | Verilen ILogger, IRedactionCallback ve IOcrConnector örnekleriyle RedactorSettings sınıfının yeni bir örneğini başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [logger](/redaction/python-net/groupdocs.redaction.options/redactorsettings/logger/) | Olayları ve hataları kaydetmek için kullanılan logger. [`ILogger`](/redaction/python-net/groupdocs.redaction.options/ilogger/) arayüzünü uygulayan bir sınıfın örneği olmalıdır. |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.options/redactorsettings/ocr_connector/) | `[`IOcrConnector`]`(/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/) arayüzünü uygulayan OCR bağlayıcı örneği. |
| [redaction_callback](/redaction/python-net/groupdocs.redaction.options/redactorsettings/redaction_callback/) | Her kırpma açıklamasını değerlendirmek için kullanılan kırpma geri çağırma. |

### Örnek

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

### Ayrıca Bakınız
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
