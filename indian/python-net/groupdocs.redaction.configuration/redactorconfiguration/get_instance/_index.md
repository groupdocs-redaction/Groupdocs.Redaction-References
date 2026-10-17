---
title: "get_instance मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "बिल्ट‑इन फ़ॉर्मेट्स की डिफ़ॉल्ट कॉन्फ़िगरेशन के साथ एक सिंगलटन इंस्टेंस लौटाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

बिल्ट‑इन फ़ॉर्मेट्स की डिफ़ॉल्ट कॉन्फ़िगरेशन के साथ एक सिंगलटन इंस्टेंस लौटाता है।

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### उदाहरण

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# सिंगलटन कॉन्फ़िगरेशन प्राप्त करें
config = RedactorConfiguration.get_instance()

# सादा टेक्स्ट फ़ॉर्मेट्स के लिए समर्थित एक्सटेंशन को विस्तारित करें
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### संबंधित देखें
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
