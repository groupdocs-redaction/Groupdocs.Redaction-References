---
title: "Redacciones de anotaciones"
linkTitle: "Annotation redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra la implementación de la redacción de anotaciones para documentos de diferentes formatos como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros."
type: docs
url: /es/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


Con la API de GroupDocs.Redaction puede aplicar redacciones de anotaciones para documentos de diferentes formatos como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros. Consulte la lista completa en el artículo [formatos de documento compatibles]().

GroupDocs.Redactions ofrece una API flexible que permite eliminar datos sensibles del texto de anotaciones, o eliminar completamente las anotaciones mediante una expresión regular.

## Remove annotations (comments etc)

Puede usar GroupDocs.Redaction para eliminar todos o ciertos comentarios y otras anotaciones del documento. Por ejemplo, podemos eliminar todos los comentarios del documento que contengan textos como "use", "show" o "describe" en su cuerpo:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Especifique las opciones de redacción para eliminar anotaciones que coincidan con el patrón
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Cargue el documento que será redactado
    with Redactor("./annotated.xlsx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(a_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` es el archivo de ejemplo utilizado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) para descargarlo.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Puede usar el constructor sin argumentos para eliminar todas las anotaciones dentro del documento.

## Redact annotations

En lugar de eliminar todas o anotaciones específicas, puedes eliminar datos sensibles del texto de la anotación. Por ejemplo, podemos eliminar todas las menciones de "John" en el documento dado, p.e.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Especifique las opciones de redacción: patrón de búsqueda y cadena de reemplazo
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Cargue el documento que será redactado
    with Redactor("./annotated.xlsx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(a_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` es el archivo de ejemplo utilizado en este caso. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) para descargarlo.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
