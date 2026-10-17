---
title: "PageRangeFilter sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belge içinde redaksiyon uygulanacak sayfa aralığını ayarlayan redaksiyon filtresini temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

Belge içinde redaksiyon uygulanacak sayfa aralığını ayarlayan redaksiyon filtresini temsil eder.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

PageRangeFilter türü aşağıdaki üyeleri ortaya çıkar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | Yeni bir RemovePageRedaction başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | Kaldırılacak sayfa sayısı. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | Başlangıç konumu indeksi (0 tabanlı). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | Arama referans konumu, belgenin başlangıcı ya da sonu. |

### Örnek

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# Son sayfayı ve ondan bir önceki sayfayı hedefleyen bir filtre tanımlayın
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# Filtre, diğer filtrelerle birleştirilebilir, ör. PageAreaFilter,
# ve bir redaksiyon yapılandırılırken ReplacementOptions.Filters'a geçirilir.
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
