---
title: "PageInfo क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "संक्षिप्त पेज जानकारी को दर्शाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

संक्षिप्त पेज जानकारी को दर्शाता है।

और अधिक जानें:
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | पृष्ठ की ऊँचाई। |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | पृष्ठ संख्या। |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | पृष्ठ की चौड़ाई। |

### उदाहरण

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

### संबंधित देखें
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
