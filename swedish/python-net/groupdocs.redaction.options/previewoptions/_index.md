---
title: "PreviewOptions-klass"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Tillhandahåller alternativ för att ange krav och ström-delegater för generering av förhandsgranskning."
type: docs
url: /sv/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Tillhandahåller alternativ för att ange krav och ström-delegater för generering av förhandsgranskning.

Klassen tillåter att specificera förhandsgranskningsformat, bilddimensioner, sidnummer och delegater som skapar och eventuellt frigör strömmar för varje genererad sida.

PreviewOptions-typen exponerar följande medlemmar:

### Konstruktörer
| Konstruktor | Beskrivning |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initierar en ny PreviewOptions-instans. Utdataströmmen kommer att stängas efter användning. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initierar en ny PreviewOptions-instans, vilket gör att utdataströmmen returneras till klienten för vidare användning. |

### Egenskaper
| Egenskap | Beskrivning |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Delegaten för skapande av sidström. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Sidans förhandsgranskningshöjd. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Sidnumren för att generera förhandsgranskning. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Formatet för förhandsgranskningsbild. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Delegaten för slutförande av sidans förhandsgranskning. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Sidans förhandsgranskningsbredd. |

### Exempel

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Skapa en fil för förhandsgranskningsbilden för den angivna sidan
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

### Se även
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
