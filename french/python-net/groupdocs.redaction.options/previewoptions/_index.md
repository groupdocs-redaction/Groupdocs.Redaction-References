---
title: "Classe PreviewOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus."
type: docs
url: /fr/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus.

La classe permet de spécifier le format d’aperçu, les dimensions de l’image, les numéros de page, ainsi que les délégués qui créent et libèrent éventuellement les flux pour chaque page générée.

Le type PreviewOptions expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | Initialise une nouvelle instance de PreviewOptions. Le flux de sortie sera fermé après utilisation. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | Initialise une nouvelle instance de PreviewOptions, faisant en sorte que le flux de sortie soit renvoyé au client pour une utilisation ultérieure. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | Le délégué de création du flux de page. |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | La hauteur de l'aperçu de page. |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | Les numéros de page pour générer l'aperçu. |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | Le format de l'image d'aperçu. |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | Le délégué de fin d'aperçu de page. |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | La largeur de l'aperçu de page. |

### Exemple

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # Créer un fichier pour l'image d'aperçu de la page donnée
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

### Voir aussi
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
