---
title: "get_document_info メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "サイズやページ数など、ドキュメントの一般情報を取得します。"
type: docs
url: /ja/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

サイズやページ数など、ドキュメントの一般情報を取得します。

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| 例外 | 説明 |
| :- | :- |
| `PasswordRequiredException` | ドキュメントがパスワードで保護されているときにスローされます。 |
| `IncorrectPasswordException` | 無効なパスワードが提供されたときにスローされます。 |

### 例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### 関連項目
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
