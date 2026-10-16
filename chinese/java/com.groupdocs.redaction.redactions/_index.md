---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "该包提供用于不同类型编辑的类。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.redaction.redactions/
---

该包提供用于不同类型编辑的类。



## 类

| 类 | 描述 |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | 表示一种编辑，它替换匹配给定正则表达式的批注文本（注释等）。 |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | 表示一种文本编辑，它替换电子表格文档（CSV、Excel 等）中的文本。 |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | 提供将 CellColumnRedaction 的范围限制在工作表和列的选项。 |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | 提供 [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) 的输入数据。 |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | 表示由 [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) 返回的结果。 |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | 表示一种文本编辑，如果文本匹配给定的正则表达式则删除批注（可选地删除所有批注）。 |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | 表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。 |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | 表示一种文本编辑，默认情况下不区分大小写地替换文档文本中的确切短语。 |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | 表示一种编辑，在图像文档的指定区域放置彩色矩形。 |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | 表示最常见的文档元数据类型列表。 |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | 表示文档元数据编辑的基础抽象类。 |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | 表示使用正则表达式搜索并编辑元数据的元数据编辑，匹配键和/或值。 |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | 表示编辑过滤器，设置文档页面内的区域以应用编辑。 |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | 表示影响页面区域内文本、图像和注释的复杂文本编辑。 |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | 表示编辑过滤器，设置文档内部的页范围以应用编辑。 |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | 表示在编辑过程中执行的单个更改操作信息。 |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | 表示编辑过滤器，设置文档内部的范围以应用编辑。 |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | 表示受编辑影响的文档数据类型。 |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | 表示通过匹配提供的正则表达式搜索并替换文档中文本的文本编辑。 |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | 表示图像区域替换的颜色和区域参数。 |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | 表示从文档中删除页面（幻灯片、工作表等）的编辑。 |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | 表示匹配文本替换的选项。 |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | 表示文档文本编辑的基础抽象类。 |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | 表示文本替换信息。 |

## 接口

| 接口 | 描述 |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | 定义自定义编辑回调。 |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | 定义获取每次编辑更改信息并可选阻止其所需的方法。 |

## 枚举

| 枚举 | 描述 |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | 提供表示文档中查找参考点的字段。 |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | 表示可用于执行编辑的操作。 |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | 表示匹配文本的替换类型。 |
