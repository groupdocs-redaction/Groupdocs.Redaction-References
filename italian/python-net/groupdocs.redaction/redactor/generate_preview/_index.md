---
title: "metodo generate_preview"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Genera immagini di anteprima di pagine specifiche in un formato immagine specificato."
type: docs
url: /it/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Genera immagini di anteprima di pagine specifiche in un formato immagine specificato.

L'anteprima è generata in base alle impostazioni definite in `preview_options`, che includono il formato immagine, le dimensioni, l'intervallo di pagine e le callback per creare e rilasciare i flussi di pagina.

```python
def generate_preview(self, preview_options):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Proprietà dell'immagine e impostazioni dell'intervallo di pagine. |

### Esempio

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Restituisce un flusso di file scrivibile per l'immagine di anteprima della pagina specificata.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Chiamato dopo che l'immagine di anteprima è stata scritta.
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

### Vedi anche
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
