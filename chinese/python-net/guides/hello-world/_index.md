---
title: "你好，世界！"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "通过创建并运行一个简单示例，快速入门 GroupDocs.Redaction for Python via .NET。"
type: docs
url: /zh/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
在探索 GroupDocs.Redaction for Python via .NET 时，\"Hello, World!\" 示例通常是第一步。它作为一个简单的测试，用于确认您的开发环境已正确设置且库能够按预期工作。

## Overview
GroupDocs.Redaction for Python via .NET 让您能够在各种文档格式中搜索、编辑和删除敏感信息。广泛的[支持的格式](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/)使其在不同用例中具有多功能性。

## How to redact a document
以下步骤演示了如何使用 GroupDocs.Redaction for Python via .NET 对文档中的敏感信息进行编辑：

1. 导入所需的 `groupdocs.redaction` 类。
2. 描述编辑（此处，将精确短语替换为彩色框）。
3. 实例化一个[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)，并提供示例文档的路径。
4. 应用编辑。
5. 保存结果。

## Complete example
下面的示例将短语 \"John Doe\" 的每一次出现替换为半透明红色框，并保存编辑后的文档：

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # 在每个 \"John Doe\" 出现处绘制半透明红色框
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # 加载文档，应用编辑，并保存结果
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` 是本示例使用的示例文件。点击[此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx)下载。

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

此示例将结果光栅化为名为 `sample_redacted.pdf` 的 PDF，因此编辑后的内容无法恢复（`save()` 默认将结果光栅化为 PDF；`redacted_file_suffix` 选项仅控制输出名称）。若想保留原始格式，请将 `rasterize_to_pdf = False` 设置为 false。

## Additional resources
此演示引用了 GroupDocs.Redaction for Python via .NET 的[代码示例](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/)。
