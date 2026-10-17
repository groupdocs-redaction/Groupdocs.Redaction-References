---
title: "PageAreaRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Sayfanın bir alanındaki metin, görüntü ve ek açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

Sayfanın bir alanındaki metin, görüntü ve ek açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder.

Daha fazla bilgi edinin

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | Yeni bir PageAreaRedaction örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | Yeni bir PageAreaRedaction başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | RegionReplacementOptions seçenekleri renk ve alan parametreleriyle. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Metin değiştirme türünü belirten [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) örneği. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Kırpmanın açıklaması, adını ve parametrelerini içerir. ([`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) üzerinden devralınmıştır) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Grafik içerikten metin çıkarmak için kullanılan IOcrConnector uygulaması. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | Eşleştirme için kullanılan düzenli ifade deseni. ([`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) üzerinden devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
