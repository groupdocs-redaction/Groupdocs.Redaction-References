---
title: "from_extension मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है।

```python
def from_extension(cls, extension):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| extension | `str` | फ़ाइल एक्सटेंशन (जिसमें अवधि "." शामिल है)। |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| उठाता है | विवरण |
| :- | :- |
| `ValueError` | जब `extension` null या खाली स्ट्रिंग हो। |

### संबंधित देखें
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
