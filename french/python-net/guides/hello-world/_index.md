---
title: "Bonjour, le monde!"
linkTitle: "Hello, World!"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Commencez rapidement avec GroupDocs.Redaction for Python via .NET en créant et exécutant un exemple simple."
type: docs
url: /fr/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Un exemple "Hello, World!" est souvent la première étape lors de l'exploration de GroupDocs.Redaction for Python via .NET. Il sert de test simple pour confirmer que votre environnement de développement est correctement configuré et que la bibliothèque fonctionne comme prévu.

## Overview
GroupDocs.Redaction for Python via .NET vous permet de rechercher, de censurer et de supprimer des informations sensibles de divers formats de documents. Une large gamme de [formats pris en charge](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) le rend polyvalent pour différents cas d'utilisation.

## How to redact a document
Les étapes suivantes montrent comment censurer des informations sensibles d'un document en utilisant GroupDocs.Redaction for Python via .NET:

1. Importez les classes `groupdocs.redaction` dont vous avez besoin.
2. Décrivez la censure (ici, une phrase exacte à remplacer par une boîte colorée).
3. Instanciez un [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) avec le chemin vers le document d'exemple.
4. Appliquez la censure.
5. Enregistrez le résultat.

## Complete example
L'exemple ci-dessous remplace chaque occurrence de la phrase "John Doe" par une boîte rouge semi-transparente et enregistre le document censuré :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Dessinez une boîte rouge semi-transparente sur chaque occurrence de "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Chargez le document, appliquez la censure et enregistrez le résultat
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) pour le télécharger.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Cet exemple rasterise le résultat en un PDF nommé `sample_redacted.pdf`, de sorte que le contenu censuré ne puisse pas être récupéré (`save()` rasterise en PDF par défaut; l'option `redacted_file_suffix` ne contrôle que le nom de sortie). Pour conserver le format original à la place, définissez `rasterize_to_pdf = False`.

## Additional resources
Cette démo fait référence aux [exemples de code](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) de GroupDocs.Redaction for Python via .NET.
