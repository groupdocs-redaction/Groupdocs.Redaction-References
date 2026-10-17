---
title: "generate_preview methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Genereert voorbeeldafbeeldingen van specifieke pagina's in een opgegeven afbeeldingsformaat."
type: docs
url: /nl/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Genereert voorbeeldafbeeldingen van specifieke pagina's in een opgegeven afbeeldingsformaat.

De preview wordt geproduceerd volgens de instellingen die zijn gedefinieerd in `preview_options`, die onder andere beeldformaat, afmetingen, paginabereik en callbacks voor het maken en vrijgeven van paginastromen omvatten.

```python
def generate_preview(self, preview_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Afbeeldingseigenschappen en paginabereikinstellingen. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Retourneert een beschrijfbare bestandsstroom voor de preview‑afbeelding van de opgegeven pagina.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Aangeroepen nadat de preview‑afbeelding is weggeschreven.
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

### Zie ook
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
