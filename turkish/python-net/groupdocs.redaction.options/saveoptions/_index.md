---
title: "SaveOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Çıktı dosya adını değiştirme ve/veya belgeyi görüntü‑tabanlı PDF'ye (tarama) dönüştürme seçeneklerini sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Çıktı dosya adını değiştirme ve/veya belgeyi görüntü‑tabanlı PDF'ye (tarama) dönüştürme seçeneklerini sağlar.

Daha fazla bilgi:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

SaveOptions türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Varsayılan ayarlarla yeni bir örnek başlatır: rasterize_to_pdf Yanlış ve add_suffix Yanlış. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Verilen parametrelerle yeni bir örnek başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | add_suffix özelliği, dosya adının kaydetmeden önce değiştirilip değiştirilmediğini gösterir. Varsayılan değer Yanlış. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | Rasterleştirme ayarları. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | Belgedeki tüm sayfaların görüntülere dönüştürülüp tek bir PDF dosyasında birleştirilip birleştirilmeyeceğini gösteren bayrak. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Çıktı dosya adı için özel ek. Belirtilmezse, [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) sabiti kullanılır. |

### Alanlar
| Alan | Açıklama |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Varsayılan ek değerini temsil eder, bu "Redacted" dir. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Belgeyi varsayılan seçeneklerle kaydet (PDF'ye rasterleştir ve ek ekle)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
`SaveOptions` kullanan görev kılavuzları:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Ayrıca Bakınız
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
