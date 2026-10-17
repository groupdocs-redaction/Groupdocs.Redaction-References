---
title: "get_document_info yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belge hakkında, boyut ve sayfa sayısı gibi genel bilgileri alır."
type: docs
url: /tr/python-net/groupdocs.redaction/redactor/get_document_info/
is_root: false
weight: 1070
---


## get_document_info

Belge hakkında, boyut ve sayfa sayısı gibi genel bilgileri alır.

```python
def get_document_info(self):
    ...
```

**Returns:** IDocumentInfo: General document information.

| Yükseltir | Açıklama |
| :- | :- |
| `PasswordRequiredException` | Belge şifre korumalı olduğunda ortaya çıkar. |
| `IncorrectPasswordException` | Geçersiz bir şifre sağlandığında ortaya çıkar. |

### Örnek

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

### Ayrıca Bakınız
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
