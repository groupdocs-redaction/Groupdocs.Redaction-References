---
title: "RegexRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder.

Daha fazla bilgi edinin

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

RegexRedaction türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | RegexRedaction'ın yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | Yeni bir RegexRedaction örneğini başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Redaction'ın adını ve parametrelerini içeren açıklama. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Eşleştirme için kullanılan düzenli ifade deseni. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Metin değiştirme türünü belirten [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) örneği. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Grafik içerikten metin çıkarmak için kullanılan IOcrConnector uygulaması. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # metinle değiştir
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # mavi katı dikdörtgenle değiştir
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
`RegexRedaction` kullanan görev kılavuzları:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
