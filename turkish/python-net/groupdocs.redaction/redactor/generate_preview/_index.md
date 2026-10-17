---
title: "generate_preview yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli sayfaların ön izleme görüntülerini verilen bir görüntü formatında oluşturur."
type: docs
url: /tr/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Belirli sayfaların ön izleme görüntülerini verilen bir görüntü formatında oluşturur.

Ön izleme, `preview_options` içinde tanımlanan ayarlara göre oluşturulur; bu ayarlar görüntü formatı, boyutlar, sayfa aralığı ve sayfa akışlarını oluşturma ve serbest bırakma geri çağrımlarını içerir.

```python
def generate_preview(self, preview_options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Görüntü özellikleri ve sayfa aralığı ayarları. |

### Örnek

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Verilen sayfanın ön izleme görüntüsü için yazılabilir bir dosya akışı döndürür.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Ön izleme görüntüsü yazıldıktan sonra çağrılır.
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Ayrıca Bakınız
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
