---
title: "__init__ yapıcı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yeni bir örnek, varsayılan ayarlarla başlatılır: rasterizetopdf False ve addsuffix False."
type: docs
url: /tr/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

Varsayılan ayarlarla yeni bir örnek başlatır: rasterize_to_pdf Yanlış ve add_suffix Yanlış.

```python
def __init__(self):
    ...
```

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

Verilen parametrelerle yeni bir örnek başlatır.

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, eğer belgedeki tüm sayfalar görüntülere dönüştürülüp tek bir PDF dosyasına yerleştirilecekse. |
| suffix | `str` | Bu metin dosya adının sonuna eklenecek; boş değilse ayrıca `add_suffix` değerini True olarak ayarlar. |

### Örnek

```python
from groupdocs.redaction.options import SaveOptions

# Varsayılan ayarlarla kaydetme seçenekleri oluşturun
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### Ayrıca Bakınız
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
