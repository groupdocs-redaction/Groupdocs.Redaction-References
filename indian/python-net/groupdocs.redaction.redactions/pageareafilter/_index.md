---
title: "PageAreaFilter वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "रिडैक्शन फ़िल्टर को दर्शाता है, जो दस्तावेज़ के पृष्ठ के भीतर एक क्षेत्र निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

रिडैक्शन फ़िल्टर को दर्शाता है, जो दस्तावेज़ के पृष्ठ के भीतर एक क्षेत्र निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।

और अधिक जानें

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | किसी विशिष्ट क्षेत्र को रिडैक्ट करने के लिए नया PageAreaFilter प्रारंभ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | पृष्ठ पर आयत (ऊपरी-बाएँ स्थिति और क्षेत्र का आकार)। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
