---
title: "RasterizationOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Dosyaları PDF'ye dönüştürmek için seçenekler sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

Dosyaları PDF'ye dönüştürmek için seçenekler sağlar.

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

RasterizationOptions türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | Yeni bir örnek başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | Uygulanacak gelişmiş bir rasterleştirme seçeneği kaydeder. |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | Uygulanacak gelişmiş bir rasterleştirme seçeneği kaydeder. |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | PDF uyumluluk seviyesi. |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | Etkinleştirme bayrağı, belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasına yerleştirilip yerleştirildiğini gösterir. Varsayılan olarak True; rasterleştirmeyi önlemek için False olarak ayarlayın. |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | Gelişmiş rasterleştirme seçenekleri ayarlandıysa gösterge True olur. |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | PDF'ye dönüştürülecek sayfa sayısı. |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | PDF'ye dönüştürülecek ilk sayfanın (0 tabanlı) indeksi. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
