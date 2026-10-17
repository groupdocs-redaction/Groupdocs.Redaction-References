---
title: "find_format मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दिए गए फ़ाइल एक्सटेंशन के लिए फ़ॉर्मेट कॉन्फ़िगरेशन खोजता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

दिए गए फ़ाइल एक्सटेंशन के लिए फ़ॉर्मेट कॉन्फ़िगरेशन खोजता है।

```python
def find_format(self, file_extension):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_extension | `str` | फ़ाइल एक्सटेंशन, फ़ॉर्मेट है ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### उदाहरण

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# सिंगलटन कॉन्फ़िगरेशन इंस्टेंस प्राप्त करें
config = RedactorConfiguration.get_instance()

# किसी दिए गए एक्सटेंशन के लिए फ़ॉर्मेट सेटिंग्स प्राप्त करें
settings = config.find_format(".txt")
if settings:
    # हैंडल किए गए एक्सटेंशन की सूची को विस्तारित करें, उदाहरण के लिए, .dump जोड़ें
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### संबंधित देखें
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
