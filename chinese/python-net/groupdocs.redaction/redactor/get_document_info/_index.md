---
title: "get_document_info 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "检索文档的一般信息，例如大小和页数。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

检索文档的一般信息，例如大小和页数。

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| 引发 | 描述 |
| :- | :- |
| `PasswordRequiredException` | 当文档受密码保护时抛出。 |
| `IncorrectPasswordException` | 当提供无效密码时抛出。 |

### 示例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### 另请参阅
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
