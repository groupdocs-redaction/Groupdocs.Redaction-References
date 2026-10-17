---
title: "get_supported_file_types メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "サポートされているファイルタイプを取得します。"
type: docs
url: /ja/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

サポートされているファイルタイプを取得します。

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### 例

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

### 関連項目
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
