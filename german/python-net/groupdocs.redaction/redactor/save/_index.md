---
title: "Speichermethode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = True, RasterizeToPDF = True."
type: docs
url: /de/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = True, RasterizeToPDF = True.

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### Beispiel

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

Speichert das Dokument in einer Datei.

```python
def save(self, save_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| save_options | `SaveOptions` | Optionen zum Hinzufügen eines Suffixes oder zum Rastern. |

**Returns:** Path to redacted document.

### Beispiel

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # Geben Sie die Redaktionsoptionen an
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wende die Schwärzung an
        redactor.apply(ex_red)

        # Speichern Sie das redigierte Dokument in seinem ursprünglichen Format mit einem Datums‑Suffix
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

Speichert das Dokument in einen Stream, einschließlich benutzerdefiniertem Speicherort.

```python
def save(self, document, rasterization_options):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| document | `io.RawIOBase` | Ziel-Stream. |
| rasterization_options | `RasterizationOptions` | Optionen zum Rastern oder Nicht‑Rastern sowie zum Angeben von Seiten für das Rastern. |

### Beispiel

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # Rasterisierung konfigurieren, um nur die erste Folie zu verarbeiten
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # Das BytesIO-Objekt enthält jetzt das gespeicherte Dokument
    data = stream.getvalue()
```

### Siehe auch
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
