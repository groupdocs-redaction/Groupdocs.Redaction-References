---
title: "save 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用以下选项将文档保存到文件：AddSuffix = True，RasterizeToPDF = True。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

使用以下选项将文档保存到文件：AddSuffix = True，RasterizeToPDF = True。

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

将文档保存到文件。

```python
def save(self, save_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| save_options | `SaveOptions` | 添加后缀或光栅化的选项。 |

**Returns:** Path to redacted document.

### 示例

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # 指定脱敏选项
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 加载待编辑的文档
    with Redactor("./sample.docx") as redactor:
        # 应用编辑
        redactor.apply(ex_red)

        # 将已编辑的文档以原始格式保存，并添加日期后缀
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

将文档保存到流，包括自定义位置。

```python
def save(self, document, rasterization_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| document | `io.RawIOBase` | 目标流。 |
| rasterization_options | `RasterizationOptions` | 是否光栅化以及指定光栅化页面的选项。 |

### 示例

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # 配置光栅化，仅处理第一张幻灯片
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # BytesIO 对象现在包含已保存的文档
    data = stream.getvalue()
```

### 另请参阅
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
