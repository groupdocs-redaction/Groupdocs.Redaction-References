---
title: "Klasse PreviewOptions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Optionen bereit, um Anforderungen und Stream‑Delegaten für die Generierung von Vorschauen festzulegen."
type: docs
url: /de/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Stellt Optionen bereit, um Anforderungen und Stream‑Delegaten für die Generierung von Vorschauen festzulegen.

Die Klasse ermöglicht die Angabe des Vorschaueformats, der Bildabmessungen, der Seitenzahlen sowie Delegaten, die für jede erzeugte Seite Streams erstellen und optional freigeben.

Der Typ PreviewOptions stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initialisiert eine neue PreviewOptions-Instanz. Der Ausgabestream wird nach der Verwendung geschlossen. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initialisiert eine neue PreviewOptions-Instanz, wodurch der Ausgabestream dem Client für weitere Verwendung zurückgegeben wird. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Der Delegat zur Erstellung des Seitenstreams. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | Die Höhe der Seitenvorschau. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Die Seitenzahlen, für die eine Vorschau erzeugt werden soll. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Das Format des Vorschau‑Bildes. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Der Delegat für den Abschluss der Seitenvorschau. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | Die Breite der Seitenvorschau. |

### Beispiel

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Erstelle eine Datei für das Vorschau‑Bild der angegebenen Seite
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

### Siehe auch
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
