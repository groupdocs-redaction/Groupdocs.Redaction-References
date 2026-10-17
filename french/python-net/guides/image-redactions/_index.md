---
title: "Redactions d'images"
linkTitle: "Image redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment masquer les données de nature sensible provenant d'images de différents formats tels que JPG, PNG, TIFF et autres."
type: docs
url: /fr/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions propose un ensemble de fonctionnalités pour masquer les données de nature sensible provenant d'images de différents formats tels que JPG, PNG, TIFF et autres. Voir la liste complète dans l'article [supported document formats]().

GroupDocs.Redaction prend en charge deux méthodes de masquage des images, à la fois dans des fichiers image séparés et dans les images incorporées :
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction pour Python via .NET vous permet également de modifier les métadonnées d'image (par ex. modifier les données EXIF d'une image ou agir comme un « effaceur EXIF »).

## Redact image area

Pour masquer une zone d'image, vous devez utiliser la classe [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) :

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Définissez la position en haut à gauche de la zone à masquer
    sample_point = Point(385, 485)
    # Définissez la taille de la zone qui doit être masquée
    sample_size = Size(1793, 2069)
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Spécifiez les options de redaction
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.jpg") as redactor:
        # Appliquer le masquage
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Par défaut, le document redacté est enregistré au format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) pour le télécharger.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Si le masquage ne peut pas être appliqué à ce type de fichiers, par ex. un document MS Word sans images incorporées, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sera [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

L'exemple suivant montre comment modifier les données EXIF (les effacer) d'une photo ou de toute autre image :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Spécifiez les options de masquage pour supprimer toutes les métadonnées d'image (par ex. EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Chargez l'image à masquer
    with Redactor("./sample.jpg") as redactor:
        # Appliquer le masquage
        result = redactor.apply(er_opt)

        # Enregistrez l'image censurée à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) pour le télécharger.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Si le masquage ne peut pas être appliqué à ce type de fichiers, par ex. une image BMP, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sera [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Vous pouvez masquer une zone d'image dans tous les types d'images incorporées à l'intérieur d'un document.

L'exemple suivant montre comment masquer toutes les images incorporées dans un document Microsoft Word :

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Définissez la position en haut à gauche de la zone à masquer
    sample_point = Point(516, 311)
    # Définissez la taille de la zone qui doit être masquée
    sample_size = Size(170, 35)
    # Définir la couleur de la boîte de rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Spécifiez les options de redaction
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquez le masquage à toutes les images incorporées
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Par défaut, le document redacté est enregistré au format PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Si le masquage ne peut pas être appliqué à ce type de fichiers, par ex. un document de feuille de calcul, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sera [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Vous pouvez supprimer des cadres d'une image multi-cadres avec une origine et un nombre de cadres donnés. Pour plus d'informations, consultez l'article [remove page redactions]().

Certains formats d'image, comme les documents DjVu, nécessitent une [pre-rasterization]() et un enregistrement ultérieur au format PDF.
