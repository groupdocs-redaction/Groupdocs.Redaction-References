---
title: "classe LoadOptions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Fournit des options qui seront utilisées pour ouvrir un fichier."
type: docs
url: /fr/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Fournit des options qui seront utilisées pour ouvrir un fichier.

En savoir plus
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

Le type LoadOptions expose les membres suivants :

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initialise une nouvelle instance de la classe LoadOptions. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initialise une nouvelle instance de LoadOptions avec le mot de passe spécifié. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initialise une nouvelle instance de LoadOptions avec le drapeau de pré‑rasterisation spécifié. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initialise une nouvelle instance de LoadOptions avec le mot de passe spécifié. |

### Propriétés
| Propriété | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Le mot de passe pour les documents protégés par mot de passe. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | Le drapeau pre_rasterize indiquant si le fichier doit être pré‑rasterisé. |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Spécifiez les options de chargement avec le mot de passe du document
load_opt = LoadOptions("mypassword")

# Définir une rédaction
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Ouvrir le document protégé par mot de passe
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Enregistrer le document rédigé
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Voir aussi
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
