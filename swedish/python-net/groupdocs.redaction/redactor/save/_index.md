---
title: "save metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Sparar dokumentet till en fil med följande alternativ: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /sv/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Sparar dokumentet till en fil med följande alternativ: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Exempel

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

Sparar dokumentet till en fil.

```python
def save(self, save_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| save_options | `SaveOptions` | Alternativ för att lägga till suffix eller rasterisera. |

**Returns:** Path to redacted document.

### Exempel

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Ange redigeringsalternativen
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera maskeringen
        redactor.apply(ex_red)

        # Spara det redigerade dokumentet i dess ursprungliga format med ett datum‑suffix
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

Sparar dokumentet till en ström, inklusive anpassad plats.

```python
def save(self, document, rasterization_options):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| document | `io.RawIOBase` | Målsström. |
| rasterization_options | `RasterizationOptions` | Alternativ för att rasterisera eller inte samt ange sidor för rasterisering. |

### Exempel

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # konfigurera rasterisering för att endast bearbeta den första bilden
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # BytesIO‑objektet innehåller nu det sparade dokumentet
    data = stream.getvalue()
```

### Se även
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
