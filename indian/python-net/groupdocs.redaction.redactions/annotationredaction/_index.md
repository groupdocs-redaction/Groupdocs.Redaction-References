---
title: "AnnotationRedaction क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक रेडैक्शन का प्रतिनिधित्व करता है जो दिए गए नियमित अभिव्यक्ति से मेल खाने वाले एनोटेशन टेक्स्ट (टिप्पणियाँ आदि) को बदलता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/annotationredaction/
is_root: false
weight: 10
---


## AnnotationRedaction class

एक रेडैक्शन का प्रतिनिधित्व करता है जो दिए गए नियमित अभिव्यक्ति से मेल खाने वाले एनोटेशन टेक्स्ट (टिप्पणियाँ आदि) को बदलता है।

और अधिक जानें

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

AnnotationRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#pattern-replacement) | एक regex पैटर्न और प्रतिस्थापन पाठ के साथ नया AnnotationRedaction प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/#regex-replacement) | [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) का नया उदाहरण प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/description/) | रेडैक्शन का विवरण, जो रेडैक्शन और उसके पैरामीटरों को वर्णित करता है। |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/expression/) | मेल खाने के लिए नियमित अभिव्यक्ति। |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/replacement/) | मिलते हुए पाठ के लिए पाठ्य प्रतिस्थापन। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import AnnotationRedaction

with Redactor("document.pdf") as redactor:
    redactor.apply(AnnotationRedaction("(?i)approved", "[REVIEW]"))
    redactor.save()
```

### Guides
`AnnotationRedaction` का उपयोग करने वाले कार्य गाइड:

* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
