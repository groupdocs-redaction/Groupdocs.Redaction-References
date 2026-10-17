---
title: "Redactor 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示控制文档编辑过程的主类，允许打开、编辑和保存文档。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

表示控制文档编辑过程的主类，允许打开、编辑和保存文档。

了解更多
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Redactor 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | 使用文件路径初始化新的 Redactor 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | 使用流初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | 使用路径为受密码保护的文档初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | 使用路径和设置为受密码保护的文档初始化新的 Redactor 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | 使用流为受密码保护的文档初始化新的 Redactor 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | 使用流和设置为受密码保护的文档初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | 对文档应用一次编辑。 |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | 对文档应用一组编辑。 |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | 对文档应用编辑策略。 |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | 释放资源。 |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | 生成特定页面的预览图像，使用给定的图像格式。 |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | 检索文档的一般信息，例如大小和页数。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | 使用以下选项将文档保存到文件：AddSuffix = True，RasterizeToPDF = True。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | 将文档保存到文件。 |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | 将文档保存到流，包括自定义位置。 |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# 打开文档并删除第一页
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
使用 `Redactor` 的任务指南：

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### 另请参阅
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
