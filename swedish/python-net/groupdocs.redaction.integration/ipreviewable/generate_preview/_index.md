---
title: "generate_preview metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat."
type: docs
url: /sv/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Genererar förhandsgranskningsbilder av specifika sidor i ett givet bildformat.

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### Se även
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
