---
title: "generate_preview Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat."
type: docs
url: /de/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Siehe auch
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
