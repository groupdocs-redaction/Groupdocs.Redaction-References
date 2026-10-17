---
title: "CellColumnRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir elektronik tablo belgesindeki (CSV, Excel, vb.) metni değiştiren bir metin kırpmasını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Bir elektronik tablo belgesindeki (CSV, Excel, vb.) metni değiştiren bir metin kırpmasını temsil eder.

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

CellColumnRedaction türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Yeni bir CellColumnRedaction başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | Redaction'ın adını ve parametrelerini içeren açıklama. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | Sütun ve çalışma sayfası filtresi. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | Eşleştirmek için düzenli ifade deseni. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Metin değiştirme türünü belirten [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) örneği. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Grafik içerikten metin çıkarmak için kullanılan IOcrConnector uygulaması. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
