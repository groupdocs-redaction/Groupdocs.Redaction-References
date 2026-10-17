---
title: "from_extension 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "将文件扩展名映射到文件类型。"
type: docs
url: /zh/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

将文件扩展名映射到文件类型。

```python
def from_extension(cls, extension):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| extension | `str` | 文件扩展名（包括句点 "."）。 |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| 引发 | 描述 |
| :- | :- |
| `ValueError` | 当 `extension` 为 null 或空字符串时。 |

### 另请参阅
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
