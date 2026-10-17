---
title: "Redacciones de metadatos"
linkTitle: "Metadata redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Este artículo muestra cómo la API de redacción de Python le permite reemplazar o eliminar metadatos usando filtros o búsqueda mediante expresiones regulares."
type: docs
url: /es/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Con la API de GroupDocs.Redaction puede aplicar redacciones de metadatos a documentos de diferentes formatos como PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX y otros. Consulte la lista completa en el artículo [formatos de documento compatibles]().

GroupDocs.Redactions ofrece una API flexible que permite reemplazar o eliminar metadatos usando filtros o búsqueda mediante expresiones regulares.

## Filter metadata

Funcionalidad base para todas las redacciones, derivada de la clase base [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) es *filtrado de metadatos* y es obligatoria para las redacciones de metadatos. Utiliza la enumeración con banderas [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), que contiene elementos para las entradas de metadatos más frecuentes. Puede establecer el filtro a *All*, o cualquier combinación de metadatos. Por ejemplo, el siguiente ejemplo establece el filtro a *Author*, *Manager* y *NameOfApplication* - para redacción textual o su limpieza:

```python
# redacción derivada de MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

A continuación se muestra la tabla con la lista completa de los elementos de [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Filtro | Valor numérico | Descripción |
| --- | --- | --- |
| *None* | 0 | Configuración de filtro vacío, no coincide con ningún elemento de metadatos |
| *Author* | 1 | Autor del documento |
| *Categoría* | 2 | Categoría del documento |
| *Comentarios* | 4 | Comentario del documento |
| *Empresa* | 8 | Empresa del autor |
| *ContentStatus* | 16 | Estado del contenido |
| *CreatedTime* | 32 | Hora de creación |
| *HyperlinkBase* | 64 | Base de hipervínculo |
| *LastPrinted* | 128 | Fecha y hora de la última impresión |
| *LastSavedBy* | 256 | Último guardado por el usuario |
| *LastSavedTime* | 1024 | Fecha y hora del último guardado |
| *NameOfApplication* | 2048 | Nombre de la aplicación donde se creó el documento |
| *Manager* | 4096 | Nombre del gerente del autor |
| *RevisionNumber* | 8192 | Número de revisión |
| *Subject* | 16384 | Asunto del documento |
| *Template* | 32768 | Nombre de la plantilla del documento |
| *Title* | 65536 | Título del documento |
| *TotalEditingTime* | 131072 | Tiempo total de edición |
| *Versión* | 262144 | Versión del documento |
| *Descripción* | 524288 | Descripción del documento |
| *Palabras clave* | 1048576 | Palabras clave del documento |
| *ContentType* | 2097152 | Tipo de contenido |
| *Todo* | 2147483647 | Todos los tipos de elementos de metadatos |

## Clean metadata

Puede reemplazar todos o algunos metadatos en el documento con valores vacíos (en blanco o mínimos) usando la clase [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/). El ejemplo a continuación elimina el contenido de todas las propiedades del documento:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Especifique las opciones de redacción para eliminar todos los metadatos
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(met_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` es el archivo de muestra utilizado en este ejemplo. Haga clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Puede especificar [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) o usar el constructor predeterminado para eliminar todos los metadatos dentro del documento especificado, Custom - para borrar todas las entradas de metadatos personalizados.

## Redact metadata

Puede usar [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) para eliminar datos sensibles de los metadatos del documento mediante expresiones regulares. Por ejemplo, podemos eliminar cualquier mención de "Company Ltd.":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Especifique las opciones de redacción: patrón de búsqueda y cadena de reemplazo
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(met_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` es el archivo de muestra utilizado en este ejemplo. Haga clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

El primer argumento es una expresión regular, el segundo es una cadena de reemplazo. También puede establecer el alcance de la redacción configurando un filtro, por ejemplo a [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - dejará sin aplicar las coincidencias de expresiones regulares en todos los elementos de metadatos, excepto la propiedad "Company":

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Especifique las opciones de redacción: patrón de búsqueda y cadena de reemplazo
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Limite el alcance de la redacción solo al elemento de metadatos Company
    met_red.filter = MetadataFilters.COMPANY

    # Cargue el documento que será redactado
    with Redactor("./sample.docx") as redactor:
        # Aplicar la redacción
        result = redactor.apply(met_red)

        # Guarde el documento redactado junto al archivo fuente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` es el archivo de muestra utilizado en este ejemplo. Haga clic en [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Todas las redacciones de metadatos se aplican a cada elemento de metadatos por separado, y aunque la redacción de un elemento falle, el resto de los elementos de metadatos se actualizará. Puede encontrar una lista de elementos de metadatos fallidos, omitidos (rechazados) y sus razones en la propiedad [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) de [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
