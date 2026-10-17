---
title: "RedactionPolicy sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Uygulanacak belirli redaksiyonların bir kümesini içeren bir temizlik politikasını temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Uygulanacak belirli redaksiyonların bir kümesini içeren bir temizlik politikasını temsil eder.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

RedactionPolicy türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Yeni bir RedactionPolicy örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Belirli bir redaksiyon listesiyle yeni bir RedactionPolicy başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Bir XML dosyasından RedactionPolicy yükler. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | XML yapılandırması içeren bir akıştan RedactionPolicy örneği yükler. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Redaksiyon politikasını bir dosyaya kaydeder. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Redaksiyon politikasını bir akışa kaydeder. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | Tamamen yapılandırılmış [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-türevi sınıfların listesi. |

### Örnek

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Bellekte yeniden kullanılabilir bir politika oluşturun
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Politikayı bir belgeye uygulayın
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
`RedactionPolicy` kullanan görev kılavuzları:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
