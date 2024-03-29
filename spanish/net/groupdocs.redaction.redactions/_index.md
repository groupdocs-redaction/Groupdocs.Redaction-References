---
title: GroupDocs.Redaction.Redactions
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: ElRedactions El espacio de nombres proporciona clases para diferentes tipos de redacciones.
type: docs
weight: 70
url: /es/net/groupdocs.redaction.redactions/
---
ElRedactions El espacio de nombres proporciona clases para diferentes tipos de redacciones.

## Clases

| Clase | Descripción |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Representa una redacción que reemplaza el texto de la anotación (comentarios, etc.) que coincide con una expresión regular determinada. |
| [CellColumnRedaction](./cellcolumnredaction) | Representa una redacción de texto que reemplaza texto en documentos de hoja de cálculo (CSV, Excel, etc.). |
| [CellFilter](./cellfilter) | Proporciona una opción para limitar el alcance de un[`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) a una hoja de trabajo y una columna. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Representa una redacción de texto que elimina las anotaciones si el texto coincide con la expresión regular dada (opcionalmente, elimina todas las anotaciones). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Representa una redacción de metadatos que borra todos los metadatos o metadatos que coincidan con MetadataFilters específicos del documento. |
| [ExactPhraseRedaction](./exactphraseredaction) | Representa una redacción de texto que reemplaza la frase exacta en el texto del documento, no distingue entre mayúsculas y minúsculas de manera predeterminada. |
| [ImageAreaRedaction](./imagearearedaction) | Representa una redacción que coloca un rectángulo de color en un área determinada de un documento de imagen. |
| [MetadataRedaction](./metadataredaction) | Representa una clase abstracta básica para la redacción de metadatos de documentos. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Representa una redacción de metadatos que busca y redacta metadatos usando expresiones regulares, claves coincidentes y/o valores. |
| [RedactionDescription](./redactiondescription) | Representa la información de una sola acción de cambio que se realizó durante el proceso de redacción. |
| [RegexRedaction](./regexredaction) | Representa una redacción de texto que busca y reemplaza texto en el documento haciendo coincidir la expresión regular proporcionada. |
| [RegionReplacementOptions](./regionreplacementoptions) | Representa los parámetros de color y área para el reemplazo de la región de la imagen. Ver[`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction) . |
| [RemovePageRedaction](./removepageredaction) | Representa una redacción que elimina una página (diapositiva, hoja de trabajo, etc.) de un documento. |
| [ReplacementOptions](./replacementoptions) | Representa opciones para el reemplazo de texto coincidente. |
| [TextRedaction](./textredaction) | Representa una clase abstracta base para redacciones de texto de documentos. |
| [TextReplacement](./textreplacement) | Representa una información de reemplazo textual. |
## Interfaces

| Interfaz | Descripción |
| --- | --- |
| [IRedactionCallback](./iredactioncallback) | Define los métodos que se requieren para recibir información sobre cada cambio de redacción y, opcionalmente, evitarlo. |
## Enumeración

| Enumeración | Descripción |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Representa una lista de los tipos más comunes de metadatos de documentos. |
| [PageSeekOrigin](./pageseekorigin) | Proporciona los campos que representan puntos de referencia en un documento para buscar. |
| [RedactionActionType](./redactionactiontype) | Representa las acciones que se pueden realizar para realizar la redacción. |
| [RedactionType](./redactiontype) | Representa un tipo de dato del documento, afectado por la redacción. |
| [ReplacementType](./replacementtype) | Representa un tipo de reemplazo del texto coincidente. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
