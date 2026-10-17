---
title: "méthode generate_preview"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Génère des images d’aperçu de pages spécifiques dans un format d’image donné."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

Génère des images d’aperçu de pages spécifiques dans un format d’image donné.

```python
def generate_preview(self, preview_options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| preview_options | `PreviewOptions` | Propriétés de l'image et paramètres de plage de pages. |

### Exemple

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

### Voir aussi
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
