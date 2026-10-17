---
title: "groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "groupdocs.redaction.redactions 下的类型。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


位于 `groupdocs.redaction.redactions` 的类型。

### 类
| 类 | 描述 |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | 表示一种编辑，它用给定正则表达式匹配的内容替换注释文本（评论等）。 |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | 表示一种文本编辑，它替换电子表格文档（CSV、Excel 等）中的文本。 |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | 提供一个选项，将 [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) 的范围限制在工作表和列上。 |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | 提供自定义编辑处理的上下文。 |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | 表示自定义编辑操作的结果。 |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | 表示一种文本编辑，如果文本匹配给定的正则表达式，则删除注释（可选地删除所有注释）。 |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | 表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。 |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | 表示一种文本编辑，默认情况下不区分大小写地替换文档文本中的确切短语。 |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | 提供一个用于实现自定义编辑逻辑的接口。 |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | 定义获取每个编辑更改信息所需的方法，并可选择性地阻止它。 |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | 表示一种在图像文档的指定区域放置彩色矩形的编辑。 |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | 表示用于文档元数据编辑的基抽象类。 |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | 表示一种使用正则表达式搜索并编辑元数据的元数据编辑，可匹配键和/或值。 |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | 表示编辑过滤器，设置文档页面内的区域以应用编辑。 |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | 表示一种复杂的文本编辑，影响页面区域内的文字、图像和批注。 |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | 表示编辑过滤器，设置文档内部的页码范围以应用编辑。 |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | 表示在编辑过程中执行的单个更改操作信息。 |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | 表示一种文本编辑，通过匹配提供的正则表达式搜索并替换文档中的文本。 |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | 表示图像区域替换的颜色和区域参数。 |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | 表示一种从文档中删除页面（幻灯片、工作表等）的编辑。 |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | 表示匹配文本替换的选项。 |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | 表示用于文档文本编辑的基抽象类。 |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | 表示文本替换信息。 |

### 枚举
| 枚举类型 | 描述 |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | 表示编辑过滤器，设置文档内部的范围以应用编辑。 |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
