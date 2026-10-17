---
title: "PageInfo 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示简要的页面信息。"
type: docs
url: /zh/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

表示简要的页面信息。

了解更多：
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | 页面高度。 |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | 页面编号。 |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | 页面宽度。 |

### 示例

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### 另请参阅
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
