---
title: "元数据脱敏"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了 Python 脱敏 API 如何使用过滤器或正则表达式搜索来替换或删除元数据。"
type: docs
url: /zh/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


使用 GroupDocs.Redaction API，您可以对 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等不同格式的文档进行元数据脱敏。请参阅 [supported document formats]() 文章中的完整列表。

GroupDocs.Redactions 提供了灵活的 API，能够使用过滤器或正则表达式搜索来替换或删除元数据。

## Filter metadata

所有脱敏的基础功能来源于 [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) 基类，其核心是 *metadata filtering*，并且对元数据脱敏是强制性的。它使用标记枚举 [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)，其中包含最常见的元数据条目。您可以将过滤器设置为 *All*，或任意元数据组合。例如，下面的示例将过滤器设置为 *Author*、*Manager* 和 *NameOfApplication*——用于文本脱敏或清除这些项：

```python
# 从 MetadataRedaction 派生的脱敏
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

下面是包含全部 [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) 项目的表格：

| 过滤器 | 数值 | 描述 |
| --- | --- | --- |
| *None* | 0 | 空过滤器设置，不匹配任何元数据项 |
| *Author* | 1 | 文档的作者 |
| *类别* | 2 | 文档的类别 |
| *评论* | 4 | 文档注释 |
| *公司* | 8 | 作者的公司 |
| *内容状态* | 16 | 内容状态 |
| *创建时间* | 32 | 创建时间 |
| *超链接基址* | 64 | 超链接基址 |
| *上次打印* | 128 | 上次打印的日期和时间 |
| *最后保存者* | 256 | 上次由用户保存 |
| *LastSavedTime* | 1024 | 上次保存的日期和时间 |
| *NameOfApplication* | 2048 | 创建文档的应用程序名称 |
| *Manager* | 4096 | 作者的经理姓名 |
| *RevisionNumber* | 8192 | 修订号 |
| *Subject* | 16384 | 文档主题 |
| *Template* | 32768 | 文档模板名称 |
| *Title* | 65536 | 文档标题 |
| *TotalEditingTime* | 131072 | 总编辑时间 |
| *版本* | 262144 | 文档的版本 |
| *描述* | 524288 | 文档的描述 |
| *关键字* | 1048576 | 文档的关键字 |
| *ContentType* | 2097152 | 内容类型 |
| *全部* | 2147483647 | 所有元数据项的类型 |

## Clean metadata

您可以使用 [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) 类将文档中的全部或特定元数据替换为空（空白或最小）值。下面的示例会将文档的所有属性清空：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # 指定擦除所有元数据的编辑选项
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(met_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` 是本示例中使用的示例文件。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

您可以指定 [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) 或使用默认构造函数来清空给定文档中的所有元数据，Custom - 清除所有自定义元数据条目。

## Redact metadata

您可以使用 [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) 通过正则表达式从文档的元数据中移除敏感数据。例如，我们可以删除所有对 "Company Ltd." 的提及：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # 指定编辑选项：搜索模式和替换字符串
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(met_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` 是本示例中使用的示例文件。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

第一个参数是正则表达式，第二个参数是替换字符串。您还可以通过设置过滤器来设定编辑范围，例如设为 [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/)。- 这将在所有元数据项中保留正则表达式匹配未处理，除 "Company" 属性外：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # 指定编辑选项：搜索模式和替换字符串
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # 仅将编辑范围限制为 Company 元数据项
    met_red.filter = MetadataFilters.COMPANY

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(met_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` 是本示例中使用的示例文件。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

所有元数据编辑都会分别应用于每个元数据项，即使某个元数据项的编辑失败，其他元数据项仍会被更新。您可以在 [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) 属性的 [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) 中找到失败、跳过（被拒绝）的元数据项及其原因列表。
