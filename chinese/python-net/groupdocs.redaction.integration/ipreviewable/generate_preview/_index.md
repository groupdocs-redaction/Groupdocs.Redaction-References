---
title: "generate_preview 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "生成特定页面的预览图像，使用给定的图像格式。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

生成特定页面的预览图像，使用给定的图像格式。

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### 另请参阅
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
