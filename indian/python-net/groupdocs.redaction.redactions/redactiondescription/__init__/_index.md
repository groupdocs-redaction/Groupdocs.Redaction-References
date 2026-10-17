---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "RedactionDescription क्लास का एक नया उदाहरण प्रारंभ करता है बिना रिप्लेसमेंट जानकारी के।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/
is_root: false
weight: 10
---


## __init__ {#redaction_type-action_type-original_text}

RedactionDescription क्लास का एक नया उदाहरण प्रारंभ करता है बिना रिप्लेसमेंट जानकारी के।

```python
def __init__(self, redaction_type, action_type, original_text):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redaction_type | `RedactionType` | रेडैक्ट किए जा रहे डेटा का प्रकार। |
| action_type | `RedactionActionType` | इन डेटा पर किए जाने वाले कार्य। |
| original_text | `str` | मिलान किया गया टेक्स्ट, टिप्पणी या एनोटेशन बॉडी। |

## __init__ {#redaction_type-action_type-original_text-replacement}

RedactionDescription क्लास का एक नया उदाहरण रिप्लेसमेंट जानकारी के साथ प्रारंभ करता है।

```python
def __init__(self, redaction_type, action_type, original_text, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redaction_type | `RedactionType` | रेडैक्ट किए जा रहे डेटा का प्रकार। |
| action_type | `RedactionActionType` | इन डेटा पर किए जाने वाले कार्य। |
| original_text | `str` | मिलान किया गया टेक्स्ट, टिप्पणी या एनोटेशन बॉडी। |
| replacement | `TextReplacement` | प्रतिस्थापन टेक्स्ट, मिलान किया गया टेक्स्ट और मूल स्ट्रिंग के भीतर उसकी स्थिति। |

## __init__ {#redaction_type-action_type-image_area_replacement-image_details}

इमेज एरिया रिप्लेसमेंट जानकारी के साथ नया RedactionDescription प्रारंभ करता है।

```python
def __init__(self, redaction_type, action_type, image_area_replacement, image_details):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| redaction_type | `RedactionType` | रेडैक्ट किए जा रहे डेटा का प्रकार। |
| action_type | `RedactionActionType` | इन डेटा पर किए जाने वाले कार्य। |
| image_area_replacement | `RegionReplacementOptions` | इमेज एरिया रिप्लेसमेंट जानकारी। |
| image_details | `str` | इमेज का टेक्स्टुअल विवरण, डिफ़ॉल्ट रूप से यह एक खाली स्ट्रिंग है। |

### संबंधित देखें
* class [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/)
