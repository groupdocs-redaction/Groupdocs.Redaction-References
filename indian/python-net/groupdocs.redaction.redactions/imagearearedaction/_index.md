---
title: "ImageAreaRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक रिडैक्शन को दर्शाता है जो छवि दस्तावेज़ के निर्दिष्ट क्षेत्र में रंगीन आयत बनाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/imagearearedaction/
is_root: false
weight: 110
---


## ImageAreaRedaction class

एक रिडैक्शन को दर्शाता है जो छवि दस्तावेज़ के निर्दिष्ट क्षेत्र में रंगीन आयत बनाता है।

और अधिक जानें:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

ImageAreaRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/__init__/#top_left-options) | एक विशिष्ट आयताकार क्षेत्र को हटाने के लिए नया ImageAreaRedaction आरंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/description/) | रेडैक्शन का विवरण, जिसमें उसका नाम और पैरामीटर शामिल हैं। |
| [options](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/options/) | RegionReplacementOptions विकल्प रंग और क्षेत्र पैरामीटर के साथ। |
| [top_left](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/top_left/) | हटाने वाले क्षेत्र की ऊपर-बाएँ स्थिति। |

### उदाहरण

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Point, Size, Color

point = Point(516, 311)
size = Size(170, 35)
color = Color.from_argb(255, 0, 0, 255)  # blue
options = RegionReplacementOptions(color, size)
redaction = ImageAreaRedaction(point, options)

with Redactor("D:\\test.jpg") as redactor:
    result = redactor.apply(redaction)
    if result.status != RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`ImageAreaRedaction` का उपयोग करने वाले कार्य मार्गदर्शक:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
