---
title: "Classe SaveOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur image (rasterisation)."
type: docs
url: /fr/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur image (rasterisation).

En savoir plus :
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

Le type SaveOptions expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Initialise une nouvelle instance avec les paramètres par défaut : rasterize_to_pdf est False et add_suffix est False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Initialise une nouvelle instance avec les paramètres fournis. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | La propriété add_suffix indique si le nom de fichier doit être modifié avant l'enregistrement. La valeur par défaut est False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | Les paramètres de rasterisation. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | Le drapeau indiquant si toutes les pages du document sont converties en images et combinées en un seul fichier PDF. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Le suffixe personnalisé pour le nom du fichier de sortie. Si non spécifié, la constante [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) est utilisée. |

### Champs
| Champ | Description |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Représente la valeur du suffixe par défaut, qui est "Redacted". |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Enregistrez le document avec les options par défaut (rasteriser en PDF et ajouter le suffixe)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
Guides de tâches qui utilisent `SaveOptions` :

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Voir aussi
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
