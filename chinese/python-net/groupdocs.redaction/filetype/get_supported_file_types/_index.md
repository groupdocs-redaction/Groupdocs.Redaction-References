---
title: "get_supported_file_types 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "检索受支持的文件类型。"
type: docs
url: /zh/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

检索受支持的文件类型。

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### 示例

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # 检索受支持的文件类型集合
    supported_file_types = FileType.get_supported_file_types()

    # 按扩展名对文件类型进行排序枚举
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### 另请参阅
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
