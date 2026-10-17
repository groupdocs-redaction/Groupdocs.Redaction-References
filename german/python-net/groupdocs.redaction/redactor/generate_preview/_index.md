---
title: "generate_preview Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat."
type: docs
url: /de/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat.

Die Vorschau wird gemäß den in `preview_options` definierten Einstellungen erzeugt, die Bildformat, Abmessungen, Seitenbereich und Rückruffunktionen zum Erstellen und Freigeben von Seitenströmen umfassen.

```python
def generate_preview(self, preview_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Bild-Eigenschaften und Seitenspanne-Einstellungen. |

### Beispiel

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # Gibt einen beschreibbaren Dateistream für das Vorschaubild der angegebenen Seite zurück.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Wird aufgerufen, nachdem das Vorschaubild geschrieben wurde.
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

### Siehe auch
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
