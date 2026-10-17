---
title: "文本编辑"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文说明了 Python 编辑 API 如何帮助您轻松地从文档中编辑敏感或私人性质的数据。您可以使用精确短语或正则表达式对 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等不同格式的文档进行文本编辑。"
type: docs
url: /zh/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction 可轻松编辑文档中敏感或私人性质的数据。最常见的编辑场景是从文档中删除文本。

使用 GroupDocs.Redaction API，您可以使用精确短语或 [正则表达式](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) 对 PDF、DOC、DOCX、PPT、PPTX、XLS、XLSX 等不同格式的文档进行文本编辑。请在 [支持的文档格式]() 文章中查看完整列表。

## Use exact phrase redaction

在下面的示例中，我们进行文本编辑，将个人精确短语 "John Doe" 替换为 "\[personal\]"（或任何豁免代码）：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # 指定脱敏选项
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

默认情况下，精确短语搜索不区分大小写。若要进行区分大小写的编辑，需要使用构造函数参数和相应的公共属性：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # 启用区分大小写的匹配
    case_sensitive = True

    # 指定脱敏选项
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

如果需要在被编辑的文本上方显示彩色框，可以使用颜色而不是替换字符串。编辑将删除匹配的文本，并在被编辑文本的位置放置指定颜色的矩形框：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 指定脱敏选项
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

您可能需要对从右到左的文档（如阿拉伯语或希伯来语）进行编辑。以下示例演示如何对阿拉伯语 PDF 文档应用 ExactPhraseRedaction：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # 使用阿拉伯语短语指定编辑选项
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # 加载待编辑的文档
    with Redactor("./arabic.pdf") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` 是本示例使用的示例文件。点击[此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf)下载。

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

在幕后，“精确短语”编辑通过正则表达式实现，正则表达式是编辑的基本方法。下面的示例中，我们使用蓝色框将匹配“2 位数字，空格或无，2 位数字，再空格和 6 位数字”的任何文本编辑掉：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 指定脱敏选项
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        result = redactor.apply(reg_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` 是本示例使用的示例文件。点击 [这里](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

如果需要编辑整段文字，可能还需要使用 RegexRedaction。以下示例演示如何在 PDF 文档中编辑整段文字：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # 定义编辑框的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 指定匹配整段的编辑选项
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.pdf") as redactor:
        # 应用编辑
        result = redactor.apply(reg_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` 是本示例使用的示例文件。点击[此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf)下载。

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
