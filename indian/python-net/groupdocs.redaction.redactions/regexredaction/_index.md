---
title: "RegexRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक टेक्स्ट रिडैक्शन को दर्शाता है जो प्रदान की गई नियमित अभिव्यक्ति से मिलाकर दस्तावेज़ में टेक्स्ट को खोजता और बदलता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

एक टेक्स्ट रिडैक्शन को दर्शाता है जो प्रदान की गई नियमित अभिव्यक्ति से मिलाकर दस्तावेज़ में टेक्स्ट को खोजता और बदलता है।

और अधिक जानें

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

RegexRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | RegexRedaction का एक नया उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | एक नया RegexRedaction उदाहरण प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | रेडैक्शन का विवरण, जिसमें उसका नाम और पैरामीटर शामिल हैं। |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | मैचिंग के लिए उपयोग किया गया नियमित अभिव्यक्ति पैटर्न। |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | पाठ प्रतिस्थापन के प्रकार को निर्दिष्ट करने वाला [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) उदाहरण। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | ग्राफिक सामग्री से पाठ निकालने के लिए उपयोग किया गया IOcrConnector कार्यान्वयन। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # पाठ के साथ बदलें
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # नीले ठोस आयत के साथ बदलें
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
`RegexRedaction` का उपयोग करने वाले टास्क गाइड्स:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
