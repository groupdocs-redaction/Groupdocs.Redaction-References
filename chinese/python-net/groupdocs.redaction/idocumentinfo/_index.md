---
title: "IDocumentInfo 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "提供获取基本文档信息所需的方法。"
type: docs
url: /zh/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

提供获取基本文档信息所需的方法。

了解更多：获取文件信息 (https://docs.groupdocs.com/redaction/net/get-file-info/)。

IDocumentInfo 类型公开以下成员：

### 属性
| 属性 | 描述 |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | 文件格式描述。 |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | 总页数。 |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | 表示页面信息的 [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) 对象列表。 |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | 文档大小（字节）。 |

### 示例

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### 另请参阅
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
