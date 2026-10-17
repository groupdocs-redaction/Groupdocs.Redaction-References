---
title: "redact मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "विशिष्ट दस्तावेज़ सामग्री पर कस्टम रेडैक्शन लागू करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

विशिष्ट दस्तावेज़ सामग्री पर कस्टम रेडैक्शन लागू करता है।

वर्तमान में, यह केवल PDF के लिए समर्थित है [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

उपयोगकर्ता अपनी स्वयं की रेडैक्शन लॉजिक परिभाषित कर सकते हैं, जैसे AI-आधारित रेडैक्शन, जो सरल पैटर्न-आधारित मेथड्स से अधिक उन्नत हो सकता है।

```python
def redact(self, context):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| context | `CustomRedactionContext` | रेडैक्ट किए जाने वाले दस्तावेज़ सामग्री को संबंधित मेटाडेटा के साथ शामिल करता है। |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### संबंधित देखें
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
