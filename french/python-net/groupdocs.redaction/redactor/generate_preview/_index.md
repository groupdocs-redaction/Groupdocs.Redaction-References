---
title: "méthode generate_preview"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Génère des images d’aperçu de pages spécifiques dans un format d’image donné."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

Génère des images d’aperçu de pages spécifiques dans un format d’image donné.

L'aperçu est généré selon les paramètres définis dans `preview_options`, qui incluent le format d'image, les dimensions, la plage de pages et les rappels pour créer et libérer les flux de pages.

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

def create_page_stream(page_number):
    # Renvoie un flux de fichier inscriptible pour l'image d'aperçu de la page donnée.
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # Appelé après que l'image d'aperçu a été écrite.
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

### Voir aussi
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
