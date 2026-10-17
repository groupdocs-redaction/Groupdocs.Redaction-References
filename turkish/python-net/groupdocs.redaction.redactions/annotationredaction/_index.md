---
title: "AnnotationRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Verilen bir düzenli ifadeye uyan açıklama metnini (yorumlar, vb.) değiştiren bir kırpmayı temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

Verilen bir düzenli ifadeye uyan açıklama metnini (yorumlar, vb.) değiştiren bir kırpmayı temsil eder.

Daha fazla bilgi edinin

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

AnnotationRedaction türü aşağıdaki üyeleri ortaya çıkar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | Bir regex deseni ve değiştirme metni ile yeni bir AnnotationRedaction başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | Yeni bir [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) örneği başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | Kırpmanın açıklaması, kırpmayı ve parametrelerini tanımlar. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | Eşleşecek düzenli ifade. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | Eşleşen metin için metinsel değiştirme. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
`AnnotationRedaction` kullanan görev kılavuzları:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
