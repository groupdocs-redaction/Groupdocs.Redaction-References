---
title: "RegionReplacementOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Görüntü bölgesi değişimi için renk ve alan parametrelerini temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

Görüntü bölgesi değişimi için renk ve alan parametrelerini temsil eder.

Daha fazla bilgi:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

RegionReplacementOptions türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | Yeni bir RegionReplacementOptions örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | Verilen metne uygun boyutta yeni bir RegionReplacementOptions sınıfı örneği başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | Kırpılmış alanı doldurmak için kullanılan renk. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | Dikdörtgenin genişliği ve yüksekliği. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # Değiştirilecek alanın sol‑üst konumunu tanımlayın
    point = Point(516, 311)
    # Değiştirilecek alanın boyutunu tanımlayın
    size = Size(170, 35)
    # Değiştirme olarak katı siyah bir dikdörtgen kullanın
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`RegionReplacementOptions` kullanan görev kılavuzları:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
