---
title: "Supprimer les censures de pages"
linkTitle: "Remove page redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment supprimer les pages contenant des données sensibles de vos documents PDF, présentations et feuilles de calcul."
type: docs
url: /fr/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction permet de supprimer facilement les pages des documents PDF, les diapositives des présentations et les feuilles de calcul des documents tableur.

Avec l'API GroupDocs.Redaction, vous pouvez supprimer des pages en spécifiant la plage de pages selon leur position relative (le début ou la fin), un indice basé sur zéro et le nombre de pages à supprimer. Pour le moment, les formats pris en charge sont : PDF, présentations (Microsoft PowerPoint, OpenOffice Presentations), documents de traitement de texte (Microsoft Word, OpenOffice Texts, fichiers Rich Text), feuilles de calcul (Microsoft Excel, OpenOffice Spreadsheets, etc.) et images multi‑cadres.

## Remove page range

Dans l'exemple ci‑dessous, nous supprimons les 2ᵉ, 3ᵉ et 4ᵉ pages du document, si le document possède suffisamment de pages :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Chargez le document à censurer
    with Redactor("./multipage_sample.pdf") as redactor:
        # Obtenir les informations du document
        doc_info = redactor.get_document_info()

        # Nécessite au moins 4 pages
        if doc_info.page_count > 3:
            # Supprimer 3 pages à partir de la 2ᵉ (indice zéro 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Appliquer le masquage
            result = redactor.apply(rem_opt)

            # Enregistrez le document masqué à côté du fichier source
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) pour le télécharger.

## Remove last page

Dans certains cas, vous pourriez devoir supprimer la dernière page ou un certain nombre de pages, quel que soit le nombre de pages présent.

L'exemple suivant montre comment supprimer la dernière page d'un document :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Supprimer 1 page en comptant depuis la fin du document
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Chargez le document à censurer
    with Redactor("./multipage_sample.pdf") as redactor:
        # Obtenir les informations du document
        doc_info = redactor.get_document_info()

        # Nécessite au moins 2 pages afin que le document ne reste pas vide
        if doc_info.page_count > 1:
            # Appliquer le masquage
            result = redactor.apply(rem_opt)

            # Enregistrez le document masqué à côté du fichier source
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) pour le télécharger.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Dans le cas d'une image multi‑cadres, vous pourriez devoir supprimer un certain nombre de cadres (traités comme des « pages »).

L'exemple suivant montre comment supprimer 3 cadres d'une image GIF animée :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Supprimer les cadres à partir du 3ᵉ (indice zéro 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Charger l'image multi‑cadres à censurer
    with Redactor("./sample.gif") as redactor:
        # Obtenir les informations du document
        doc_info = redactor.get_document_info()

        # Nécessite au moins 7 cadres
        if doc_info.page_count >= 7:
            # Appliquer le masquage
            result = redactor.apply(rem_opt)

            # Enregistrez l'image censurée à côté du fichier source
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) pour le télécharger.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
