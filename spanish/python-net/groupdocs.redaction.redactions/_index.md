---
title: "groupdocs.redaction.redactions"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Tipos bajo groupdocs.redaction.redactions."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


Tipos bajo `groupdocs.redaction.redactions`.

### Clases
| Clase | Descripción |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | Representa una redacción que reemplaza el texto de anotaciones (comentarios, etc.) que coinciden con una expresión regular dada. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | Representa una redacción de texto que reemplaza el texto en un documento de hoja de cálculo (CSV, Excel, etc.). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | Proporciona una opción para limitar el alcance de un [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) a una hoja de cálculo y una columna. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | Proporciona contexto para el procesamiento de redacción personalizada. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | Representa el resultado de una operación de redacción personalizada. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | Representa una redacción de texto que elimina anotaciones si el texto coincide con una expresión regular dada (opcionalmente elimina todas las anotaciones). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | Representa una redacción de metadatos que borra todos los metadatos o los metadatos que coinciden con filtros específicos de MetadataFilters del documento. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | Representa una redacción de texto que reemplaza una frase exacta en el texto del documento, sin distinción de mayúsculas por defecto. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | Proporciona una interfaz para implementar lógica de redacción personalizada. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | Define los métodos necesarios para recibir información sobre cada cambio de redacción y, opcionalmente, evitarlo. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | Representa una redacción que coloca un rectángulo coloreado en un área determinada de un documento de imagen. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | Representa una clase abstracta base para redacciones de metadatos de documentos. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | Representa una redacción de metadatos que busca y redacta metadatos usando expresiones regulares, coincidiendo claves y/o valores. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | Representa un filtro de redacción, estableciendo un área dentro de una página de un documento para aplicar la redacción. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | Representa una redacción textual compleja que afecta texto, imágenes y anotaciones en un área de la página. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | Representa un filtro de redacción, estableciendo un rango de páginas dentro de un documento para aplicar la redacción. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | Representa la información de una única acción de cambio que se realizó durante el proceso de redacción. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Representa una redacción de texto que busca y reemplaza texto en el documento coincidiendo con la expresión regular proporcionada. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | Representa los parámetros de color y área para el reemplazo de regiones de imagen. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | Representa una redacción que elimina una página (diapositiva, hoja de cálculo, etc.) de un documento. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | Representa opciones para el reemplazo de texto coincidente. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | Representa una clase abstracta base para redacciones de texto de documentos. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | Representa información de reemplazo textual. |

### Enumeraciones
| Enumeración | Descripción |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | Representa un filtro de redacción, estableciendo el alcance dentro de un documento para aplicar redacciones. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
