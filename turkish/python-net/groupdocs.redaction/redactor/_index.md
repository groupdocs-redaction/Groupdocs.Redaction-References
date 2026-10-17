---
title: "Redactor sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belge redaksiyon sürecini kontrol eden, belgeleri açma, redakte etme ve kaydetmeye izin veren ana sınıfı temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Belge redaksiyon sürecini kontrol eden, belgeleri açma, redakte etme ve kaydetmeye izin veren ana sınıfı temsil eder.

Daha fazla bilgi edinin
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Redactor türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Bir dosya yolu kullanarak yeni bir Redactor örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | `[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` kullanarak bir akış ile yeni bir örnek başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | `[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` şifre korumalı belge için yolunu kullanarak yeni bir örnek başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Şifre korumalı bir belge için yol ve ayarları kullanarak yeni bir Redactor örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Şifre korumalı bir belge için bir akış kullanarak yeni bir Redactor örneği başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | `[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)` şifre korumalı bir belge için bir akış ve ayarları kullanarak yeni bir örnek başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Belgeye bir redaksiyon uygular. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Belgeye bir redaksiyon seti uygular. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Belgeye bir redaksiyon politikası uygular. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Kaynakları serbest bırakır. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Belirli sayfaların ön izleme görüntülerini verilen bir görüntü formatında oluşturur. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Belge hakkında, boyut ve sayfa sayısı gibi genel bilgileri alır. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Belgeyi bir dosyaya kaydeder. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Belgeyi özel konum dahil olmak üzere bir akışa kaydeder. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Bir belge aç ve ilk sayfayı kaldır
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
`Redactor` kullanan görev kılavuzları:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Ayrıca Bakınız
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
