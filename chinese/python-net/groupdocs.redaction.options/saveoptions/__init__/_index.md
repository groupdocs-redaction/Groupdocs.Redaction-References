---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用默认设置初始化新实例：rasterizetopdf 为 False，addsufix 为 False。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

使用默认设置初始化一个新实例：rasterize_to_pdf 为 False，add_suffix 为 False。

```python
def __init__(self):
    ...
```

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

使用给定参数初始化一个新实例。

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | 如果文档中的所有页面需要转换为图像并放入单个 PDF 文件，则为 True。 |
| suffix | `str` | 此文本将添加到文件名末尾；如果非空，还会将 `add_suffix` 设置为 True。 |

### 示例

```python
from groupdocs.redaction.options import SaveOptions

# 使用默认设置创建保存选项
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### 另请参阅
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
