---
title: "metodo generate_preview"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Genera immagini di anteprima di pagine specifiche in un formato immagine specificato."
type: docs
url: /it/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Genera immagini di anteprima di pagine specifiche in un formato immagine specificato.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Vedi anche
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
