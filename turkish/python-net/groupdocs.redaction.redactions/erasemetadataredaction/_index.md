---
title: "EraseMetadataRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgeden tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri kırpmasını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Belgeden tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri kırpmasını temsil eder.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

EraseMetadataRedaction türü aşağıdaki üyeleri ortaya çıkar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Tüm meta verileri silen EraseMetadataRedaction sınıfının yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Belirtilen `MetadataFilters` ile eşleşen meta verileri silen EraseMetadataRedaction sınıfının yeni bir örneğini başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Belirli bir format örneğine redaksiyonu uygular. ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Redaksiyonun ve parametrelerinin açıklaması. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Yazar veya Şirket gibi tüm veya belirli meta verileri seçmek için kullanılan filtre. ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Tüm meta verileri sil
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Yalnızca yazar alanını sil
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
`EraseMetadataRedaction` kullanan görev kılavuzları:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
