---
title: "RedactionPolicy क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक सैनिटाइज़ेशन पॉलिसी को दर्शाता है, जिसमें लागू करने के लिए विशिष्ट रेडैक्शन का सेट शामिल है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

एक सैनिटाइज़ेशन पॉलिसी को दर्शाता है, जिसमें लागू करने के लिए विशिष्ट रेडैक्शन का सेट शामिल है।

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

RedactionPolicy प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | एक नया RedactionPolicy इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | विशिष्ट रेडैक्शन सूची के साथ एक नया RedactionPolicy प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | XML फ़ाइल से एक RedactionPolicy लोड करता है। |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | XML कॉन्फ़िगरेशन वाली स्ट्रीम से एक RedactionPolicy इंस्टेंस लोड करता है। |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | रेडैक्शन नीति को फ़ाइल में सहेजता है। |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | रेडैक्शन नीति को स्ट्रीम में सहेजता है। |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | पूरी तरह कॉन्फ़िगर किए गए [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-व्युत्पन्न क्लासों की सूची। |

### उदाहरण

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# मेमोरी में पुन: उपयोग योग्य नीति बनाएं
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# नीति को दस्तावेज़ पर लागू करें
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
`RedactionPolicy` का उपयोग करने वाले टास्क गाइड्स:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
