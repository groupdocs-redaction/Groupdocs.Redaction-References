---
title: "com.groupdocs.redaction.redactions"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "El paquete proporciona clases para diferentes tipos de redacciones."
type: docs
weight: 16
url: /es/java/com.groupdocs.redaction.redactions/
---

El paquete proporciona clases para diferentes tipos de redacciones.



## Clases

| Clase | Descripción |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Representa una redacción que reemplaza el texto de anotación (comentarios, etc.) que coincide con una expresión regular dada. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Representa una redacción de texto que reemplaza el texto en documentos de hoja de cálculo (CSV, Excel, etc.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Proporciona una opción para limitar el alcance de una CellColumnRedaction a una hoja de cálculo y una columna. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Proporciona datos de entrada para [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Representa un resultado devuelto por [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Representa una redacción de texto que elimina anotaciones si el texto coincide con una expresión regular dada (opcionalmente elimina todas las anotaciones). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Representa una redacción de metadatos que borra todos los metadatos o los metadatos que coinciden con filtros específicos MetadataFilters del documento. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Representa una redacción de texto que reemplaza una frase exacta en el texto del documento, sin distinción de mayúsculas por defecto. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Representa una redacción que coloca un rectángulo de color en el área dada de un documento de imagen. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Representa una lista de los tipos de metadatos de documento más comunes. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Representa una clase abstracta base para la redacción de metadatos de documentos. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Representa una redacción de metadatos que busca y redacta metadatos usando expresiones regulares, coincidiendo claves y/o valores. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Representa un filtro de redacción, estableciendo un área dentro de una página de un documento para aplicar la redacción. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Representa una redacción textual compleja que afecta texto, imágenes y anotaciones en un área de la página. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Representa un filtro de redacción, estableciendo un rango de páginas dentro de un documento para aplicar la redacción. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Representa la información de una única acción de cambio que se realiza durante el proceso de redacción. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Representa un filtro de redacción, estableciendo el alcance dentro de un documento para aplicar redacciones. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Representa un tipo de datos del documento, afectados por la redacción. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Representa los parámetros de color y área para el reemplazo de regiones de imagen. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Representa una redacción que elimina una página (diapositiva, hoja de cálculo, etc.) de un documento. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Representa opciones para el reemplazo de texto coincidente. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Representa una clase abstracta base para redacciones de texto de documentos. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Representa información de reemplazo textual. |

## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Define una devolución de llamada personalizada para la redacción. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Define métodos que son necesarios para recibir información sobre cada cambio de redacción y, opcionalmente, prevenirlo. |

## Enumeraciones

| Enum | Descripción |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Proporciona los campos que representan puntos de referencia en un documento para la búsqueda. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Representa acciones que pueden tomarse para realizar la redacción. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Representa un tipo de reemplazo para el texto coincidente. |
