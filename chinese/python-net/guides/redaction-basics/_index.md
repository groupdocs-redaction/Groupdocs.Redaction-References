---
title: "编辑基础"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了 Python 开发者如何在文档中应用元数据、图像、批注和文本编辑。支持广泛的文档格式，如 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等。"
type: docs
url: /zh/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction 支持一套有效的文档编辑功能。它允许对[text](), [metadata](), [annotations](), [images]() 进行编辑。

支持广泛的文档格式，如：PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等。完整的支持格式列表请参见[受支持的文档格式]() 文章。

## Redaction types

GroupDocs.Redaction 包含以下编辑类型：

| 类型 | 描述 | 类 |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)，[AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

对文档进行编辑遮蔽是通过 [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) 方法完成的。结果，您会收到一个 [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) 实例，其中包含每个已应用遮蔽的日志条目。该条目包含对 [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) 实例的引用，包括其选项、操作状态（见下文）以及在适用时的文本描述。如果至少有一个遮蔽失败，您将看到 [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/)：

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # 指定脱敏选项
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # 将脱敏后的文档保存到源文件旁边
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` 是本示例中使用的示例文件。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

以下表格列出了 [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) 枚举的所有可能状态：

| 状态 | 描述 | 可能原因 |
| --- | --- | --- |
| *Applied* | 遮蔽已完全且成功地应用 | 遮蔽过程中的所有操作均已成功应用 |
| *PartiallyApplied* | 遮蔽仅对其匹配项的一部分应用 | 1) 替换的试用限制已超出2) 至少有一次更改被用户拒绝 |
| *Skipped* | 遮蔽被跳过（未应用） | 1) 遮蔽的试用限制已超出2) 遮蔽无法应用于此类文档3) 所有替换均被用户拒绝，未进行任何更改 |
| *Failed* | 遮蔽因异常而失败 | 在遮蔽过程中出现异常 |

要获取详细信息，您必须遍历 [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) 中的遮蔽日志条目，并检查状态不是 *Applied* 的任何项的 [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) 属性：

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # 默认情况下，已遮蔽的文档会以 PDF 格式保存
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # 导出所有失败或跳过的遮蔽
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

您可以在一次调用 [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) 方法时应用任意数量的遮蔽，因为其重载接受遮蔽数组和遮蔽策略。在这种情况下，遮蔽将按照它们在数组中出现的顺序依次应用。作为在代码中指定遮蔽集的替代方案，您可以创建包含遮蔽策略的 XML 文件，如 [此处]() 所述。

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 提供按顺序应用的遮蔽列表
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑列表
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # 默认情况下，已遮蔽的文档会以 PDF 格式保存
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # 导出所有失败或跳过的遮蔽
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` 是本示例中使用的示例文件。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) 下载它。

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
