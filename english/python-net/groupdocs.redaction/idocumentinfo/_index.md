---
title: IDocumentInfo class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides methods required for getting basic document information."
type: docs
url: /python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Provides methods required for getting basic document information.

Learn more: Get file info (https://docs.groupdocs.com/redaction/net/get-file-info/).

The IDocumentInfo type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | The file format description. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | The total page count. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | The list of [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) objects representing page information. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | The document size in bytes. |

### Example

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
