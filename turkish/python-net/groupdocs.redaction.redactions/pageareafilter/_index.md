---
title: "PageAreaFilter sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgenin bir sayfası içinde redaksiyon uygulanacak bir alanı ayarlayan redaksiyon filtresini temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

Belgenin bir sayfası içinde redaksiyon uygulanacak bir alanı ayarlayan redaksiyon filtresini temsil eder.

Daha fazla bilgi edinin

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | Belirli bir alanı gizlemek için yeni bir PageAreaFilter başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | Sayfadaki dikdörtgen (alanın sol üst konumu ve boyutu). |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
