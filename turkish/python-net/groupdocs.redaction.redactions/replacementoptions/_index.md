---
title: "ReplacementOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Eşleşen metin değişimi için seçenekleri temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Eşleşen metin değişimi için seçenekleri temsil eder.

Daha fazla bilgi edinin

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

ReplacementOptions türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Belirtilen değiştirme metniyle ReplacementOptions'ın yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Renkli dikdörtgeni seçenek olarak kullanarak ReplacementOptions sınıfının yeni bir örneğini başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | Değiştirme eylemi: kutu çiz veya metni değiştir. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | Bir `ReplacementType.draw_box` seçeneği için renk (aksi takdirde yok sayılır). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | Kullanıcıların kendi redaksiyon mantıklarını tanımlamasına izin veren özel redaksiyon işleyicisi. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | Bu redaksiyonla uygulanacak filtrelerin dizisi. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | Metinsel değiştirme değeri. |

### Örnek

```python
from groupdocs.redaction.redactions import ReplacementOptions

# Eşleşen metni "[X]" yer tutucusuyla değiştir.
repl_opt = ReplacementOptions("[X]")
```

### Guides
`ReplacementOptions` kullanan görev kılavuzları:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
