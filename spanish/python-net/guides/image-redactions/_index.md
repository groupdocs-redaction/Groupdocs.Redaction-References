---
title: "Redacciones de imágenes"
linkTitle: "Image redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo redactar datos de naturaleza sensible de imágenes de varios formatos como JPG, PNG, TIFF y otros."
type: docs
url: /es/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions ofrece un conjunto de funciones para redactar datos de naturaleza sensible de imágenes de varios formatos como JPG, PNG, TIFF y otros. Consulte la lista completa en el artículo [supported document formats]().

GroupDocs.Redaction admite dos formas de redactar imágenes, tanto en archivos de imagen separados como en imágenes incrustadas:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction para Python a través de .NET también permite cambiar los metadatos de la imagen (p. ej., editar datos EXIF de una imagen o actuar como un "borrador de EXIF").

## Redact image area

Para redactar un área de imagen, debes usar la clase [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Define la posición superior izquierda del área a redactar
    sample_point = Point(385, 485)
    # Define el tamaño del área que necesita ser redactada
    sample_size = Size(1793, 2069)
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Especifique las opciones de redacción
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.jpg") as redactor:
        # Aplicar la redacción
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Por defecto, el documento redactado se guarda en formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` es el archivo de ejemplo utilizado en este caso. Haz clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) para descargarlo.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Si la redacción no puede aplicarse a este tipo de archivos, p. ej., documento MS Word sin imágenes incrustadas, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) será [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

El siguiente ejemplo muestra cómo editar los datos EXIF (borrarlos) de una foto o cualquier otra imagen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Especifica las opciones de redacción para eliminar todos los metadatos de la imagen (p. ej., EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Carga la imagen que será redactada
    with Redactor("./sample.jpg") as redactor:
        # Aplicar la redacción
        result = redactor.apply(er_opt)

        # Guardar la imagen redactada junto al archivo original
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` es el archivo de ejemplo utilizado en este caso. Haz clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) para descargarlo.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Si la redacción no puede aplicarse a este tipo de archivos, p. ej., imagen BMP, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) será [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Puedes redactar áreas de imagen dentro de todo tipo de imágenes incrustadas dentro de un documento.

El siguiente ejemplo muestra cómo redactar todas las imágenes incrustadas dentro de un documento Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Define la posición superior izquierda del área a redactar
    sample_point = Point(516, 311)
    # Define el tamaño del área que necesita ser redactada
    sample_size = Size(170, 35)
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Especifique las opciones de redacción
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplica la redacción a todas las imágenes incrustadas
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Por defecto, el documento redactado se guarda en formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` es el archivo de ejemplo utilizado en este caso. Haz clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) para descargarlo.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Si la redacción no puede aplicarse a este tipo de archivos, p. ej., un documento de hoja de cálculo, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) será [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Puedes eliminar fotogramas de una imagen multifuente con un origen y número de fotogramas dados. Para información adicional, consulta el artículo [remove page redactions]().

Algunos formatos de imagen, como los documentos DjVu, requieren [pre-rasterization]() y posterior guardado en formato PDF.
