---
title: "RemovePageRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir belgeden sayfa (slayt, çalışma sayfası vb.) kaldıran bir redaksiyonu temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

Bir belgeden sayfa (slayt, çalışma sayfası vb.) kaldıran bir redaksiyonu temsil eder.

Daha fazla bilgi edinin
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | Yeni bir RemovePageRedaction başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | Kaldırılacak sayfa sayısı. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | Başlangıç konumu indeksi (0 tabanlı). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | Arama referans konumu, belgenin başlangıcı ya da sonu. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | Redaksiyonun adı ve parametrelerini içeren açıklaması. ([`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/) üzerinden devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Belgenin sonundan itibaren 1 sayfa kaldır
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(rem_opt)

        # Redakte edilmiş belgeyi kaydedin
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
`RemovePageRedaction` kullanan görev kılavuzları:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
