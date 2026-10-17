---
title: "DeleteAnnotationRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो यदि टेक्स्ट दिए गए नियमित अभिव्यक्ति से मेल खाता है तो एनोटेशन को हटाता है (वैकल्पिक रूप से सभी एनोटेशन को हटाता है)।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/deleteannotationredaction/
is_root: false
weight: 60
---


## DeleteAnnotationRedaction class

एक टेक्स्ट रेडैक्शन का प्रतिनिधित्व करता है जो यदि टेक्स्ट दिए गए नियमित अभिव्यक्ति से मेल खाता है तो एनोटेशन को हटाता है (वैकल्पिक रूप से सभी एनोटेशन को हटाता है)।

और अधिक जानें

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/

DeleteAnnotationRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/) | DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जिसमें सभी एनोटेशन को हटाने की सेटिंग्स (सब कुछ मिलान) होती हैं। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#pattern) | DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जो दिए गए अभिव्यक्ति से मेल खाने वाले एनोटेशन को हटाता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/#regex) | DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जो दिए गए अभिव्यक्ति से मेल खाने वाले एनोटेशन को हटाता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/description/) | रेडैक्शन का विवरण, जिसमें रेडैक्शन नाम और पैरामीटर शामिल हैं। |
| [expression](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/expression/) | मेल खाने के लिए नियमित अभिव्यक्ति। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

with Redactor("document.pdf") as redactor:
    # ऐसे एनोटेशन हटाएँ जिनमें शब्द "internal" (बिना केस के) शामिल हो।
    redactor.apply(DeleteAnnotationRedaction("(?i)internal"))
    redactor.save()
```

### Guides
`DeleteAnnotationRedaction` का उपयोग करने वाले कार्य मार्गदर्शक:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
