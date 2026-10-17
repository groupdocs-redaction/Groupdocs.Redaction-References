---
title: "ExactPhraseRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ के टेक्स्ट में एक सटीक वाक्यांश को बदलता है, डिफ़ॉल्ट रूप से केस-इंसेंसिटिव।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ के टेक्स्ट में एक सटीक वाक्यांश को बदलता है, डिफ़ॉल्ट रूप से केस-इंसेंसिटिव।

और अधिक जानें:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | केस‑इंसेंसिटिव मोड में ExactPhraseRedaction का एक नया उदाहरण आरंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | एक नया ExactPhraseRedaction उदाहरण आरंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | रेडैक्शन का विवरण, जिसमें रेडैक्शन नाम और पैरामीटर शामिल हैं। |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | यह मान दर्शाता है कि खोज केस‑सेंसिटिव है या नहीं। |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | पाठ दिशा संकेतक दर्शाता है कि पाठ दाएँ‑से‑बाएँ है या नहीं। डिफ़ॉल्ट रूप से False है। |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | खोजने और प्रतिस्थापित करने के लिए स्ट्रिंग। |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | पाठ प्रतिस्थापन के प्रकार को निर्दिष्ट करने वाला [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) उदाहरण। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | ग्राफिक सामग्री से पाठ निकालने के लिए उपयोग किया गया IOcrConnector कार्यान्वयन। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # केस‑सेंसिटिव प्रतिस्थापन
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
`ExactPhraseRedaction` का उपयोग करने वाले कार्य मार्गदर्शक:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
