---
title: "获取支持的文件格式"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了如何使用 Python 获取 GroupDocs.Redaction 支持的所有文件格式列表。"
type: docs
url: /zh/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction 通过以下步骤获取所有支持的文件格式列表：

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

以下示例演示如何获取支持的文件格式列表。

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

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)
