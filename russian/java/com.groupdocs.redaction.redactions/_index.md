---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Пакет предоставляет классы для различных типов замазываний."
type: docs
weight: 16
url: /ru/java/com.groupdocs.redaction.redactions/
---

Пакет предоставляет классы для различных типов замазываний.



## Классы

| Класс | Описание |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Представляет редактирование, которое заменяет текст аннотации (комментарии и т.д.), соответствующий заданному регулярному выражению. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Представляет текстовое редактирование, которое заменяет текст в электронных таблицах (CSV, Excel и т.д.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Предоставляет параметр для ограничения области действия CellColumnRedaction листом и столбцом. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Предоставляет входные данные для [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Представляет результат, возвращаемый [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Представляет текстовое редактирование, которое удаляет аннотации, если текст соответствует заданному регулярному выражению (по желанию удаляет все аннотации). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Представляет редактирование метаданных, которое стирает все метаданные или метаданные, соответствующие определённым MetadataFilters, из документа. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Представляет текстовое редактирование, которое заменяет точную фразу в тексте документа, по умолчанию без учёта регистра. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Представляет редактирование, которое размещает цветной прямоугольник в указанной области изображения документа. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Представляет список наиболее распространённых типов метаданных документа. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Представляет базовый абстрактный класс для редактирования метаданных документа. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Представляет удаление метаданных, которое ищет и удаляет метаданные с помощью регулярных выражений, сопоставляя ключи и/или значения. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Представляет сложное текстовое редактирование, которое влияет на текст, изображения и аннотации в области страницы. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Представляет информацию о единственном действии изменения, выполненном в процессе редактирования. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Представляет фильтр редактирования, задающий область внутри документа для применения редактирований. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Представляет тип данных документа, затронутый редактированием. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Представляет параметры цвета и области для замены региона изображения. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Представляет редактирование, которое удаляет страницу (слайд, лист и т.д.) из документа. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Представляет параметры для замены найденного текста. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Представляет базовый абстрактный класс для текстовых редактирований документа. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Представляет информацию о текстовой замене. |

## Интерфейсы

| Интерфейс | Описание |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Определяет пользовательский обратный вызов редактирования. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Определяет методы, необходимые для получения информации о каждом изменении редактирования и, при желании, предотвращения его. |

## Перечисления

| Перечисление | Описание |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Предоставляет поля, представляющие контрольные точки в документе для перемещения. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Представляет действия, которые можно выполнить для редактирования. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Представляет тип замены для найденного текста. |
