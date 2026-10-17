---
title: "الفئة IDocumentInfo"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يوفر طرقًا مطلوبة للحصول على معلومات أساسية عن المستند."
type: docs
url: /ar/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

يوفر طرقًا مطلوبة للحصول على معلومات أساسية عن المستند.

المزيد من المعلومات: الحصول على معلومات الملف (https://docs.groupdocs.com/redaction/net/get-file-info/).

نوع IDocumentInfo يعرض الأعضاء التالية:

### الخصائص
| خاصية | الوصف |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | وصف تنسيق الملف. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | إجمالي عدد الصفحات. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | قائمة كائنات [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) التي تمثل معلومات الصفحة. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | حجم المستند بالبايت. |

### مثال

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### انظر أيضًا
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
