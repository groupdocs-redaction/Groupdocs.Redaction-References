---
title: "PreviewOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlama seçeneklerini sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Önizleme oluşturma için gereksinimleri ve akış delegelerini ayarlama seçeneklerini sağlar.

Sınıf, ön izleme formatını, görüntü boyutlarını, sayfa numaralarını belirtmeye ve her oluşturulan sayfa için akışları oluşturan ve isteğe bağlı olarak serbest bırakan temsilcileri tanımlamaya olanak tanır.

PreviewOptions türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Yeni bir PreviewOptions örneği başlatır. Çıktı akışı kullanım sonrası kapatılacaktır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Yeni bir PreviewOptions örneği başlatır, çıktı akışının istemciye daha sonraki kullanım için geri döndürülmesine neden olur. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Sayfa akışı oluşturma temsilcisi. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Sayfa önizleme yüksekliği. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Önizleme oluşturulacak sayfa numaraları. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Önizleme görüntü formatı. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Sayfa önizleme tamamlama temsilcisi. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Sayfa önizleme genişliği. |

### Örnek

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Verilen sayfanın önizleme görüntüsü için bir dosya oluştur.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
