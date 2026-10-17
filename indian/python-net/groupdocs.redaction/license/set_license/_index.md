---
title: "set_license मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "वर्तमान प्रक्रिया में एक लाइसेंस लागू करें।"
type: docs
url: /hi/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

वर्तमान प्रक्रिया में एक लाइसेंस लागू करें।

```python
def set_license(self, license_source):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| license_source |  | या तो एक स्ट्रिंग पाथ जो ``.lic`` फ़ाइल की ओर इशारा करता है या एक पढ़ने योग्य फ़ाइल-जैसा ऑब्जेक्ट जो लाइसेंस बाइट्स देता है। फ़ाइल-जैसे इनपुट को अस्थायी फ़ाइल में लिखा जाता है इससे पहले कि उन्हें ब्रिज को पास किया जाए। |

| उठाता है | विवरण |
| :- | :- |
| `TypeError` | यदि ``license_source`` न तो स्ट्रिंग पाथ है और न ही पढ़ने योग्य फ़ाइल-जैसा ऑब्जेक्ट। |

### संबंधित देखें
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
