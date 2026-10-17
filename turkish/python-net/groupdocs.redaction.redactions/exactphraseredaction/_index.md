---
title: "ExactPhraseRedaction sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgenin metnindeki tam bir ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız şekilde değiştiren bir metin kırpmasını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Belgenin metnindeki tam bir ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız şekilde değiştiren bir metin kırpmasını temsil eder.

Daha fazla bilgi:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Büyük/küçük harfe duyarsız modda yeni bir ExactPhraseRedaction örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Yeni bir ExactPhraseRedaction örneği başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Redaction'ı verilen bir format örneğine uygular. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | Kırpma açıklaması, kırpma adını ve parametrelerini içerir. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | Aramanın büyük/küçük harfe duyarlı olup olmadığını gösteren değer. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | Metnin sağdan sola olup olmadığını gösteren yön bayrağı. Varsayılan değer False'tur. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | Aranacak ve değiştirilecek dize. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | Metin değiştirme türünü belirten [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) örneği. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | Grafik içerikten metin çıkarmak için kullanılan IOcrConnector uygulaması. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) tarafından devralınmıştır) |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # büyük/küçük harfe duyarlı değiştirme
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
`ExactPhraseRedaction` kullanan görev kılavuzları:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
