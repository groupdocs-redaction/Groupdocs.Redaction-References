---
title: "DeleteAnnotationRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Metin verilen bir düzenli ifadeye eşleşirse açıklamaları (isteğe bağlı olarak tüm açıklamaları) silen bir metin kırpmasını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

Metin verilen bir düzenli ifadeye eşleşirse açıklamaları (isteğe bağlı olarak tüm açıklamaları) silen bir metin kırpmasını temsil eder.

Daha fazla bilgi edinin

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

DeleteAnnotationRedaction türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | DeleteAnnotationRedaction sınıfının yeni bir örneğini, tüm ek açıklamaları (her şeyi eşleştiren) silmek için ayarlarla başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | DeleteAnnotationRedaction sınıfının yeni bir örneğini, verilen ifadeye uyan ek açıklamaları silerek başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | Kırpma açıklaması, kırpma adını ve parametrelerini içerir. |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | Eşleşecek düzenli ifade. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # "internal" kelimesini içeren ek açıklamaları sil (büyük/küçük harfe duyarsız)
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
`DeleteAnnotationRedaction` kullanan görev kılavuzları:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
