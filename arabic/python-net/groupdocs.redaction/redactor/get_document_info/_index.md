---
title: "طريقة get_document_info"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يسترجع المعلومات العامة حول المستند، مثل الحجم وعدد الصفحات."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

يسترجع المعلومات العامة حول المستند، مثل الحجم وعدد الصفحات.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| يُثير | الوصف |
| :- | :- |
| `PasswordRequiredException` | يُرفع عندما يكون المستند محميًا بكلمة مرور. |
| `IncorrectPasswordException` | يُرفع عندما يتم تقديم كلمة مرور غير صالحة |

### مثال

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### انظر أيضًا
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
