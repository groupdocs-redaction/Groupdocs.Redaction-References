---
title: "generate_preview 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "生成特定页面的预览图像，使用给定的图像格式。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

生成特定页面的预览图像，使用给定的图像格式。

预览根据 `preview_options` 中定义的设置生成，其中包括图像格式、尺寸、页码范围，以及用于创建和释放页面流的回调函数。

```python
def generate_preview(self, preview_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| preview_options | `PreviewOptions` | 图像属性和页面范围设置。 |

### 示例

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # 返回给定页面的预览图像的可写文件流。
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # 在预览图像写入后调用。
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### 另请参阅
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
