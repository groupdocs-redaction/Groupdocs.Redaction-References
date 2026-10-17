---
title: "注释编辑"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了针对 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等不同格式文档的注释编辑实现。"
type: docs
url: /zh/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


使用 GroupDocs.Redaction API，您可以对 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等不同格式的文档应用注释编辑。请在[支持的文档格式]()文章中查看完整列表。

GroupDocs.Redactions 提供了灵活的 API，允许从注释文本中删除敏感数据，或通过正则表达式完全删除注释。

## Remove annotations (comments etc)

您可以使用 GroupDocs.Redaction 从文档中删除所有或特定的评论和其他注释。例如，我们可以删除文档中正文包含 \"use\"、\"show\" 或 \"describe\" 等文本的所有评论：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # 指定编辑选项以删除匹配模式的注释
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # 加载待编辑的文档
    with Redactor("./annotated.xlsx") as redactor:
        # 应用编辑
        result = redactor.apply(a_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` 是本示例使用的示例文件。点击[此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)下载。

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

您可以使用无参构造函数来删除文档中的所有注释。

## Redact annotations

与其删除所有或特定的批注，您可以从批注文本中移除敏感数据。例如，我们可以删除给定文档中所有对“John”的提及，例如：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # 指定编辑选项：搜索模式和替换字符串
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # 加载待编辑的文档
    with Redactor("./annotated.xlsx") as redactor:
        # 应用编辑
        result = redactor.apply(a_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` 是本示例使用的示例文件。点击[此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx)下载。

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
