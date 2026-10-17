---
title: "save metodu"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /tr/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Belgeyi aşağıdaki seçeneklerle bir dosyaya kaydeder: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

Belgeyi bir dosyaya kaydeder.

```python
def save(self, save_options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| save_options | `SaveOptions` | Sonek ekleme veya rasterleştirme seçenekleri. |

**Returns:** Path to redacted document.

### Örnek

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        redactor.apply(ex_red)

        # Kırpılmış belgeyi orijinal formatında tarih sonekiyle kaydet
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

Belgeyi özel konum dahil olmak üzere bir akışa kaydeder.

```python
def save(self, document, rasterization_options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| document | `io.RawIOBase` | Hedef akış. |
| rasterization_options | `RasterizationOptions` | Rasterleştirip rasterleştirmeme ve rasterleştirme sayfalarını belirtme seçenekleri. |

### Örnek

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # Rasterleştirmeyi yalnızca ilk slaytı işlemek üzere yapılandır
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # BytesIO nesnesi artık kaydedilen belgeyi içeriyor
    data = stream.getvalue()
```

### Ayrıca Bakınız
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
