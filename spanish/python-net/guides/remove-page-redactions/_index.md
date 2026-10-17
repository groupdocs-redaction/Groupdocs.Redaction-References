---
title: "Eliminar redacciones de página"
linkTitle: "Remove page redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo eliminar páginas con datos sensibles de sus documentos PDF, de presentaciones y de hojas de cálculo."
type: docs
url: /es/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction permite eliminar fácilmente páginas de documentos PDF, diapositivas de presentaciones y hojas de cálculo.

Con la API de GroupDocs.Redaction puedes eliminar páginas especificando el rango de páginas mediante su posición relativa (el principio o el final), índice basado en cero y la cantidad de páginas a eliminar. En este momento los formatos compatibles son: PDF, presentaciones (Microsoft PowerPoint, OpenOffice Presentations), documentos de procesamiento de texto (Microsoft Word, OpenOffice Texts, archivos Rich Text), hojas de cálculo (Microsoft Excel, OpenOffice Spreadsheets, etc.) e imágenes de varios fotogramas.

## Remove page range

En el ejemplo a continuación, eliminamos la segunda, tercera y cuarta página del documento, si el documento tiene suficientes páginas:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Cargue el documento que será redactado
    with Redactor("./multipage_sample.pdf") as redactor:
        # Obtener información del documento
        doc_info = redactor.get_document_info()

        # Requiere al menos 4 páginas
        if doc_info.page_count > 3:
            # Eliminar 3 páginas a partir de la segunda (índice basado en cero 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Aplicar la redacción
            result = redactor.apply(rem_opt)

            # Guarde el documento redactado junto al archivo fuente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) para descargarlo.

## Remove last page

En algunos casos puede que necesite eliminar la última página o varias páginas, sin importar cuántas haya.

El siguiente ejemplo muestra cómo eliminar la última página de un documento:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Eliminar 1 página contando desde el final del documento
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Cargue el documento que será redactado
    with Redactor("./multipage_sample.pdf") as redactor:
        # Obtener información del documento
        doc_info = redactor.get_document_info()

        # Requiere al menos 2 páginas para que el documento no quede vacío
        if doc_info.page_count > 1:
            # Aplicar la redacción
            result = redactor.apply(rem_opt)

            # Guarde el documento redactado junto al archivo fuente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) para descargarlo.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

En el caso de una imagen de varios fotogramas puede que necesite eliminar varios fotogramas (tratados como "páginas").

El siguiente ejemplo muestra cómo eliminar 3 fotogramas de una imagen GIF animada:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Eliminar fotogramas a partir del tercero (índice basado en cero 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Cargar la imagen de varios fotogramas que será redactada
    with Redactor("./sample.gif") as redactor:
        # Obtener información del documento
        doc_info = redactor.get_document_info()

        # Requiere al menos 7 fotogramas
        if doc_info.page_count >= 7:
            # Aplicar la redacción
            result = redactor.apply(rem_opt)

            # Guardar la imagen redactada junto al archivo original
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` es el archivo de ejemplo usado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) para descargarlo.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
