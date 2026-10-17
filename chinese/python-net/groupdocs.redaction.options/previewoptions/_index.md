---
title: "PreviewOptions 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "提供设置预览生成的需求和流委托的选项。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

提供设置预览生成的需求和流委托的选项。

该类允许指定预览格式、图像尺寸、页码，以及用于为每个生成的页面创建并可选释放流的委托。

PreviewOptions 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | 初始化一个新的 PreviewOptions 实例。使用后输出流将被关闭。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | 初始化一个新的 PreviewOptions 实例，使输出流返回给客户端以供进一步使用。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | 页面流创建委托。 |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | 页面预览高度。 |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | 生成预览的页面编号。 |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | 预览图像格式。 |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | 页面预览完成委托。 |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | 页面预览宽度。 |

### 示例

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # 为给定页面的预览图像创建文件
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 另请参阅
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
