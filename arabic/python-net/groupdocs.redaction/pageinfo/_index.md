---
title: "الفئة PageInfo"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يمثل معلومات مختصرة عن الصفحة."
type: docs
url: /ar/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

يمثل معلومات مختصرة عن الصفحة.

المزيد:
- https://docs.groupdocs.com/redaction/net/get-file-info/

نوع PageInfo يعرض الأعضاء التالية:

### المنشئات
| منشئ | الوصف |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | ارتفاع الصفحة. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | رقم الصفحة. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | عرض الصفحة. |

### مثال

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

### انظر أيضًا
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
