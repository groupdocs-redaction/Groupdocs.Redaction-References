---
title: "PageRangeFilter क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "रिडैक्शन फ़िल्टर को दर्शाता है, जो दस्तावेज़ के भीतर पृष्ठ रेंज निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

रिडैक्शन फ़िल्टर को दर्शाता है, जो दस्तावेज़ के भीतर पृष्ठ रेंज निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

PageRangeFilter प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | एक नया RemovePageRedaction इनिशियलाइज़ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | हटाने के लिए पृष्ठों की संख्या। |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | शुरुआती स्थिति इंडेक्स (0-आधारित)। |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | सीक रेफ़रेंस पोज़िशन, जो दस्तावेज़ की शुरुआत या अंत हो सकता है। |

### उदाहरण

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# एक फ़िल्टर परिभाषित करें जो अंतिम पृष्ठ और उससे पहले वाले पृष्ठ को लक्षित करता है
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# फ़िल्टर को अन्य फ़िल्टरों के साथ संयोजित किया जा सकता है, उदाहरण के लिए, PageAreaFilter,
# और रेडैक्शन कॉन्फ़िगर करते समय ReplacementOptions.Filters को पास किया जाता है।
```

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
