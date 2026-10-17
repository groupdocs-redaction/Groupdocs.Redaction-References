---
title: "RegionReplacementOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "छवि क्षेत्र प्रतिस्थापन के लिए रंग और क्षेत्र पैरामीटर को दर्शाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

छवि क्षेत्र प्रतिस्थापन के लिए रंग और क्षेत्र पैरामीटर को दर्शाता है।

और अधिक जानें:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

RegionReplacementOptions प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | एक नया RegionReplacementOptions इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | RegionReplacementOptions क्लास का एक नया इंस्टेंस प्रारंभ करता है जिसकी आकार दिया गया टेक्स्ट से मेल खाती है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | रेडैक्टेड क्षेत्र को भरने के लिए उपयोग किया गया रंग। |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | आयत की चौड़ाई और ऊँचाई। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # प्रतिस्थापित करने वाले क्षेत्र की शीर्ष‑बाएँ स्थिति निर्धारित करें
    point = Point(516, 311)
    # प्रतिस्थापित करने वाले क्षेत्र का आकार निर्धारित करें
    size = Size(170, 35)
    # प्रतिस्थापन के रूप में एक ठोस काली आयत का उपयोग करें
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
टास्क गाइड्स जो `RegionReplacementOptions` का उपयोग करते हैं:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
