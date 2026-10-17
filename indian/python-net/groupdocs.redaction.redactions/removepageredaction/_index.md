---
title: "RemovePageRedaction वर्ग"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक रिडैक्शन को दर्शाता है जो दस्तावेज़ से एक पृष्ठ (स्लाइड, वर्कशीट, आदि) को हटाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

एक रिडैक्शन को दर्शाता है जो दस्तावेज़ से एक पृष्ठ (स्लाइड, वर्कशीट, आदि) को हटाता है।

और अधिक जानें
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | एक नया RemovePageRedaction इनिशियलाइज़ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | हटाने के लिए पृष्ठों की संख्या। |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | शुरुआती स्थिति इंडेक्स (0-आधारित)। |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | सीक रेफ़रेंस पोज़िशन, जो दस्तावेज़ की शुरुआत या अंत हो सकता है। |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | रेडैक्शन का विवरण, जिसमें इसका नाम और पैरामीटर शामिल हैं। (से विरासत में मिला [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # दस्तावेज़ के अंत से 1 पृष्ठ हटाएँ
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(rem_opt)

        # रिडैक्टेड दस्तावेज़ सहेजें
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
`RemovePageRedaction` का उपयोग करने वाले कार्य गाइड:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
