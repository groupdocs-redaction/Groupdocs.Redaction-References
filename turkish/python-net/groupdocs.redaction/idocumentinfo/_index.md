---
title: "IDocumentInfo sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Temel belge bilgilerini almayı gerektiren yöntemleri sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

Temel belge bilgilerini almayı gerektiren yöntemleri sağlar.

Daha fazla bilgi edinin: Dosya bilgilerini al (https://docs.groupdocs.com/redaction/net/get-file-info/).

IDocumentInfo türü aşağıdaki üyeleri gösterir:

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | Dosya formatı açıklaması. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | Toplam sayfa sayısı. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | Sayfa bilgilerini temsil eden [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) nesnelerinin listesi. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | Belgenin bayt cinsinden boyutu. |

### Örnek

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### Ayrıca Bakınız
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
