---
title: "generate_preview yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli sayfaların ön izleme görüntülerini verilen bir görüntü formatında oluşturur."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Belirli sayfaların ön izleme görüntülerini verilen bir görüntü formatında oluşturur.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Ayrıca Bakınız
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
