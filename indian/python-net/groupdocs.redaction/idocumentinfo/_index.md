---
title: "IDocumentInfo क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "बुनियादी दस्तावेज़ जानकारी प्राप्त करने के लिए आवश्यक मेथड्स प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

बुनियादी दस्तावेज़ जानकारी प्राप्त करने के लिए आवश्यक मेथड्स प्रदान करता है।

और अधिक जानें: फ़ाइल जानकारी प्राप्त करें (https://docs.groupdocs.com/redaction/net/get-file-info/).

IDocumentInfo प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### गुण
| गुण | विवरण |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | फ़ाइल फ़ॉर्मेट विवरण। |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | कुल पृष्ठ गिनती। |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | पृष्ठ जानकारी का प्रतिनिधित्व करने वाले [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) वस्तुओं की सूची। |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | दस्तावेज़ का आकार बाइट्स में। |

### उदाहरण

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### संबंधित देखें
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
