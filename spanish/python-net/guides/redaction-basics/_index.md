---
title: "Conceptos básicos de redacción"
linkTitle: "Redaction basics"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo los desarrolladores de Python pueden aplicar redacción de metadatos, imágenes, anotaciones y texto en sus documentos. Se admite una amplia gama de formatos de documento, como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros."
type: docs
url: /es/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction admite un conjunto eficaz de funciones de redacción de documentos. Permite aplicar redacciones para [text](), [metadata](), [annotations](), [images]().

Se admite una amplia gama de formatos de documento, como: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros. Consulte la lista completa de formatos compatibles en el artículo [supported document formats]().

## Redaction types

GroupDocs.Redaction incluye los siguientes tipos de redacción:

| Tipo | Descripción | Clases |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Aplicar la redacción a un documento se realiza mediante el método [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) . Como resultado, recibe una instancia de [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) , que contiene una entrada de registro para cada redacción aplicada. La entrada contiene una referencia a la instancia [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) , incluyendo sus opciones, el estado de la operación (ver abajo) y descripciones textuales cuando corresponda. Si al menos una redacción falla, verá [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) :

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Especifique las opciones de redacción
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Guarde el documento redactado junto al archivo fuente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` es el archivo de ejemplo usado en este ejemplo. Haga clic en [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Todos los estados posibles de la enumeración [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) se enumeran en esta tabla:

| Estado | Descripción | Razones posibles |
| --- | --- | --- |
| *Applied* | La redacción se aplicó completa y exitosamente | Todas las operaciones dentro del proceso de redacción se aplicaron con éxito |
| *PartiallyApplied* | La redacción se aplicó solo a una parte de sus coincidencias | 1) Se superaron las limitaciones de prueba para reemplazos 2) Al menos un cambio fue rechazado por el usuario |
| *Skipped* | La redacción se omitió (no se aplicó) | 1) Se superaron las limitaciones de prueba para redacciones 2) La redacción no puede aplicarse a este tipo de documento 3) Todas las sustituciones fueron rechazadas por el usuario y no se realizaron cambios |
| *Failed* | La redacción falló con una excepción | Ocurrió una excepción durante el proceso de redacción |

Para obtener información detallada debe iterar a través de las entradas del registro de redacción en [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) , y comprobar la propiedad [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) de cualquier elemento con un estado distinto de *Applied* :

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Por defecto, el documento redactado se guarda en formato PDF
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Volcar todas las redacciones fallidas o omitidas
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

Puede aplicar tantas redacciones como necesite en una sola llamada al método [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) , ya que su sobrecarga acepta una matriz de redacciones y una política de redacción. En este caso, las redacciones se aplicarán en el mismo orden en que aparecen en la matriz. Como alternativa a especificar conjuntos de redacción en su código, puede crear un archivo XML con la política de redacción, como se describe [here]().

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Definir el color del cuadro de redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Proporcione una lista de redacciones para aplicar en orden
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la lista de redacciones
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Por defecto, el documento redactado se guarda en formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Volcar todas las redacciones fallidas o omitidas
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` es el archivo de ejemplo usado en este ejemplo. Haga clic en [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) para descargarlo.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
