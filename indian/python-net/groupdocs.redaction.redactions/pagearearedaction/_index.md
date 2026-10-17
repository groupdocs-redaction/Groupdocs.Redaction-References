---
title: "PageAreaRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक जटिल टेक्स्टुअल रिडैक्शन को दर्शाता है जो पृष्ठ के एक क्षेत्र में टेक्स्ट, छवियों और एनोटेशन को प्रभावित करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

एक जटिल टेक्स्टुअल रिडैक्शन को दर्शाता है जो पृष्ठ के एक क्षेत्र में टेक्स्ट, छवियों और एनोटेशन को प्रभावित करता है।

और अधिक जानें

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | नया PageAreaRedaction उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | नया PageAreaRedaction प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | RegionReplacementOptions विकल्प रंग और क्षेत्र पैरामीटर के साथ। |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | पाठ प्रतिस्थापन के प्रकार को निर्दिष्ट करने वाला [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) उदाहरण। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | रेडैक्शन का विवरण, जिसमें इसका नाम और पैरामीटर शामिल हैं। (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | ग्राफिक सामग्री से पाठ निकालने के लिए उपयोग किया गया IOcrConnector कार्यान्वयन। ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) से विरासत में मिला) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | मैचिंग के लिए उपयोग किया गया रेगुलर एक्सप्रेशन पैटर्न। (inherited from [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
