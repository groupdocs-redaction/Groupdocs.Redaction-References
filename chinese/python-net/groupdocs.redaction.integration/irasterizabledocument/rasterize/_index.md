---
title: "rasterize 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "将文档保存为 PDF 并写入流。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

将文档保存为 PDF 并写入流。

```python
def rasterize(self, output):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| output | `io.RawIOBase` | 目标流。 |

## rasterize {#output-options}

将文档保存为 PDF 并写入流，可指定页面范围和合规性选项。

```python
def rasterize(self, output, options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| output | `io.RawIOBase` | 目标流。 |
| options | `RasterizationOptions` | PDF 转换选项。 |

### 另请参阅
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
