---
title: "recognize 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "对以流形式提供的图像执行 OCR 处理。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration.ocr/iocrconnector/recognize/
is_root: false
weight: 1010
---


## recognize {#image_stream}

对以流形式提供的图像执行 OCR 处理。

```python
def recognize(self, image_stream):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | 包含要处理图像的流。 |

**Returns:** Structured recognized text, containing lines, words and their bounding rectangles.

### 另请参阅
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/)
