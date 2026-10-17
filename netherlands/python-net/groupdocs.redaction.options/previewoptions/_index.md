---
title: "PreviewOptions klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt opties om vereisten en stream‑delegates in te stellen voor het genereren van een voorbeeld."
type: docs
url: /nl/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Biedt opties om vereisten en stream‑delegates in te stellen voor het genereren van een voorbeeld.

De klasse maakt het mogelijk om het voorbeeldformaat, de afbeeldingsafmetingen, paginanummers en delegaten die streams maken en eventueel vrijgeven voor elke gegenereerde pagina te specificeren.

Het type PreviewOptions exposeert de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initialiseert een nieuwe PreviewOptions‑instantie. De uitvoerstroom wordt na gebruik gesloten. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initialiseert een nieuwe PreviewOptions‑instantie, waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | De delegate voor het maken van de paginastroom. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | De hoogte van de paginavoorvertoning. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | De paginanummers om een voorvertoning te genereren. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Het formaat van de voorvertoningsafbeelding. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | De delegate voor het voltooien van de paginavoorvertoning. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | De breedte van de paginavoorvertoning. |

### Voorbeeld

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Maak een bestand voor de voorvertoningsafbeelding van de opgegeven pagina.
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

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
