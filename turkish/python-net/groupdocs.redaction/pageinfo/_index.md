---
title: "PageInfo sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Kısa bir sayfa bilgisini temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

Kısa bir sayfa bilgisini temsil eder.

Daha fazla bilgi:
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo türü aşağıdaki üyeleri sunar:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | Sayfa yüksekliği. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | Sayfa numarası. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | Sayfa genişliği. |

### Örnek

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

### Ayrıca Bakınız
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
