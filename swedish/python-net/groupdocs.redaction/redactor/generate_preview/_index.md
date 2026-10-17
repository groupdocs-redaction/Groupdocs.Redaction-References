---
title: "generate_preview metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat."
type: docs
url: /sv/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat.

Förhandsgranskningen genereras enligt inställningarna definierade i `preview_options`, som inkluderar bildformat, dimensioner, sidintervall samt återuppringningar för att skapa och släppa sidströmmar.

```python
def generate_preview(self, preview_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Bildegenskaper och sidintervallinställningar. |

### Exempel

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Returnerar en skrivbar filström för förhandsgranskningsbilden för den angivna sidan.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Anropas efter att förhandsgranskningsbilden har skrivits.
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

### Se även
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
