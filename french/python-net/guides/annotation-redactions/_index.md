---
title: "Censures d'annotations"
linkTitle: "Annotation redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre l'implémentation de la censure d'annotations pour des documents de différents formats tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres."
type: docs
url: /fr/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Avec l'API GroupDocs.Redaction, vous pouvez appliquer des censures d'annotations pour des documents de différents formats tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres. Voir la liste complète dans l'article [formats de documents pris en charge]().

GroupDocs.Redactions fournit une API flexible qui permet de supprimer les données sensibles du texte des annotations, ou de supprimer complètement les annotations à l'aide d'une expression régulière.

## Remove annotations (comments etc)

Vous pouvez utiliser GroupDocs.Redaction pour supprimer tous les commentaires ou des commentaires spécifiques ainsi que d'autres annotations du document. Par exemple, nous pouvons supprimer tous les commentaires du document contenant des textes tels que "use", "show" ou "describe" dans leur corps :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Spécifiez les options de censure pour supprimer les annotations correspondant au modèle
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Chargez le document à censurer
    with Redactor("./annotated.xlsx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(a_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) pour le télécharger.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Vous pouvez utiliser le constructeur sans arguments pour supprimer toutes les annotations du document.

## Redact annotations

Au lieu de supprimer toutes les annotations ou des annotations spécifiques, vous pouvez supprimer les données sensibles du texte de l'annotation. Par exemple, nous pouvons supprimer toutes les mentions de "John" dans le document donné, par ex. :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Spécifiez les options de rédaction : motif de recherche et chaîne de remplacement
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Chargez le document à censurer
    with Redactor("./annotated.xlsx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(a_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) pour le télécharger.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
