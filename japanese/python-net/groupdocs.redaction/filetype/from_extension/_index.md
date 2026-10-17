---
title: "from_extension メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ファイル拡張子をファイルタイプにマッピングします。"
type: docs
url: /ja/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

ファイル拡張子をファイルタイプにマッピングします。

```python
def from_extension(cls, extension):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| extension | `str` | ファイル拡張子（ピリオド「.」を含む）。 |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| 例外 | 説明 |
| :- | :- |
| `ValueError` | `extension` が null または空文字列の場合。 |

### 関連項目
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
