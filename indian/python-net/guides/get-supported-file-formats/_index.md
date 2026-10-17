---
title: "समर्थित फ़ाइल फ़ॉर्मैट प्राप्त करें"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दिखाता है कि Python का उपयोग करके GroupDocs.Redaction के सभी समर्थित फ़ाइल फ़ॉर्मैट की सूची कैसे प्राप्त करें।"
type: docs
url: /hi/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction इन चरणों के द्वारा सभी समर्थित फ़ाइल फ़ॉर्मैट की सूची प्राप्त करने की अनुमति देता है:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

निम्नलिखित उदाहरण दिखाता है कि समर्थित फ़ाइल फ़ॉर्मैट सूची कैसे प्राप्त करें।

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # समर्थित फ़ाइल प्रकारों का संग्रह प्राप्त करें
    supported_file_types = FileType.get_supported_file_types()

    # फ़ाइल प्रकारों को एक्सटेंशन के अनुसार क्रमबद्ध करके सूचीबद्ध करें
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)
