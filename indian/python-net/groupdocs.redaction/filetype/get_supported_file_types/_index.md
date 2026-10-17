---
title: "get_supported_file_types मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "समर्थित फ़ाइल प्रकारों को प्राप्त करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

समर्थित फ़ाइल प्रकारों को प्राप्त करता है।

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### उदाहरण

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

### संबंधित देखें
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
