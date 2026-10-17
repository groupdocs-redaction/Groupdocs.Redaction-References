---
title: "MetadataSearchRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Anahtarları ve/veya değerleri eşleştirerek düzenli ifadelerle meta veriyi arayan ve redakte eden bir meta veri redaksiyonunu temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

Anahtarları ve/veya değerleri eşleştirerek düzenli ifadelerle meta veriyi arayan ve redakte eden bir meta veri redaksiyonunu temsil eder.

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | MetadataSearchRedaction sınıfının yeni bir örneğini, kırpılmış öğeleri eşleştirmek için değer kullanarak başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | MetadataSearchRedaction'ın yeni bir örneğini, kırpılmış öğeleri eşleştirmek için öğe adı ve değer kullanarak başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | MetadataSearchRedaction sınıfının yeni bir örneğini, kırpılmış öğeleri eşleştirmek için değer kullanarak başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | MetadataSearchRedaction'ın yeni bir örneğini, kırpılmış öğeleri eşleştirmek için öğe adı ve değer kullanarak başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Belirli bir format örneğine redaksiyonu uygular. ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | Redaction'ın adını ve parametrelerini içeren açıklama. |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | Bir meta veri öğesinin adını (anahtarını) eşleştirmek için düzenli ifade. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | Metinsel değiştirme değeri. |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | Bir meta veri öğesinin değer metnini eşleştirmek için düzenli ifade. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Yazar veya Şirket gibi tüm veya belirli meta verileri seçmek için kullanılan filtre. ([`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) üzerinden devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Desene uyan herhangi bir meta veri değerini kırp.
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
`MetadataSearchRedaction` kullanan görev kılavuzları:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
