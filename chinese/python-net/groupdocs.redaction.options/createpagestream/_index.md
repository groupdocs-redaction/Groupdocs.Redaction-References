---
title: "CreatePageStream 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示一个返回用于写入页面预览数据的流的方法。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/createpagestream/
is_root: false
weight: 20
---


## CreatePageStream class

表示一个返回用于写入页面预览数据的流的方法。

CreatePageStream 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/createpagestream/__init__/#object-method) |  |

### 方法
| 方法 | 描述 |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke/#page_number-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke_int32/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke/#page_number) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke_int32/) |  |

### 示例

```python
import os
import io
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int) -> io.RawIOBase:
    page_path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(page_path, "wb")

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 另请参阅
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
