---
title: "save methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Slaat het document op in een bestand met de volgende opties: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /nl/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Slaat het document op in een bestand met de volgende opties: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Voorbeeld

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

Slaat het document op in een bestand.

```python
def save(self, save_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| save_options | `SaveOptions` | Opties om een achtervoegsel toe te voegen of te rasteren. |

**Returns:** Path to redacted document.

### Voorbeeld

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Specificeer de redactie‑opties
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe
        redactor.apply(ex_red)

        # Sla het geredigeerde document op in het oorspronkelijke formaat met een datumachtervoegsel.
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

Slaat het document op in een stream, inclusief aangepaste locatie.

```python
def save(self, document, rasterization_options):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| document | `io.RawIOBase` | Doelstream. |
| rasterization_options | `RasterizationOptions` | Opties om al dan niet te rasteren en om pagina's voor rasteren op te geven. |

### Voorbeeld

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # configureer rasteren om alleen de eerste dia te verwerken.
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # het BytesIO object bevat nu het opgeslagen document
    data = stream.getvalue()
```

### Zie ook
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
