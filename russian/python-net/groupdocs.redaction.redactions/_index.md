---
title: "groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Типы в groupdocs.redaction.redactions."
type: docs
url: /ru/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


Типы в `groupdocs.redaction.redactions`.

### Классы
| Класс | Описание |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | Представляет редактирование, которое заменяет текст аннотации (комментарии и т.п.), соответствующий заданному регулярному выражению. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | Представляет текстовое редактирование, которое заменяет текст в таблице (CSV, Excel и т.д.). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | Предоставляет возможность ограничить область действия [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) листом и столбцом. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | Предоставляет контекст для пользовательской обработки редактирования. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | Представляет результат пользовательской операции редактирования. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | Представляет текстовое редактирование, которое удаляет аннотации, если текст соответствует заданному регулярному выражению (опционально удаляет все аннотации). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | Представляет редактирование метаданных, которое стирает все метаданные или метаданные, соответствующие определённым MetadataFilters, из документа. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | Представляет текстовое редактирование, которое заменяет точную фразу в тексте документа, без учёта регистра по умолчанию. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | Предоставляет интерфейс для реализации пользовательской логики редактирования. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | Определяет методы, необходимые для получения информации о каждом изменении редактирования и, при необходимости, предотвращения его. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | Представляет редактирование, которое размещает цветной прямоугольник в заданной области изображения документа. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | Представляет базовый абстрактный класс для редактирования метаданных документа. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | Представляет редактирование метаданных, которое ищет и редактирует метаданные с помощью регулярных выражений, сопоставляя ключи и/или значения. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | Представляет сложное текстовое редактирование, которое влияет на текст, изображения и аннотации в области страницы. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | Представляет фильтр редактирования, задающий диапазон страниц внутри документа для применения редактирования. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | Представляет информацию о единственном действии изменения, выполненном в процессе редактирования. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | Представляет параметры цвета и области для замены региона изображения. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | Представляет редактирование, которое удаляет страницу (слайд, лист, и т.д.) из документа. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | Представляет параметры для замены найденного текста. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | Представляет базовый абстрактный класс для редактирования текста документа. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | Представляет информацию о текстовой замене. |

### Перечисления
| Перечисление | Описание |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | Представляет фильтр редактирования, задающий область внутри документа для применения редактирований. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
