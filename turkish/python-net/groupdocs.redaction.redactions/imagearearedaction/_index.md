---
title: "ImageAreaRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir görüntü belgesinin belirli bir alanına renkli bir dikdörtgen yerleştiren bir redaksiyonu temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

Bir görüntü belgesinin belirli bir alanına renkli bir dikdörtgen yerleştiren bir redaksiyonu temsil eder.

Daha fazla bilgi:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

ImageAreaRedaction türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | Belirli bir dikdörtgen alanı gizlemek için yeni bir ImageAreaRedaction başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | Redaction'ın adını ve parametrelerini içeren açıklama. |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | RegionReplacementOptions seçenekleri renk ve alan parametreleriyle. |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | Kaldırılacak alanın sol üst konumu. |

### Örnek

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`ImageAreaRedaction` kullanan görev kılavuzları:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
