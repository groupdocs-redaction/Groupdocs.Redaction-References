---
title: "サポートされているファイル形式を取得する"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、Python を使用して GroupDocs.Redaction のすべてのサポート対象ファイル形式の一覧を取得する方法を示します。"
type: docs
url: /ja/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction は、以下の手順でサポートされているすべてのファイル形式の一覧を取得できます：

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

以下の例は、サポートされているファイル形式の一覧を取得する方法を示しています。

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # サポートされているファイルタイプのコレクションを取得する
    supported_file_types = FileType.get_supported_file_types()

    # 拡張子でソートされたファイルタイプを列挙する
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
