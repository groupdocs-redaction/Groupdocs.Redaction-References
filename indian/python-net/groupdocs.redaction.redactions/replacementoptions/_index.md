---
title: "ReplacementOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "मिलाए गए टेक्स्ट प्रतिस्थापन के विकल्पों को दर्शाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

मिलाए गए टेक्स्ट प्रतिस्थापन के विकल्पों को दर्शाता है।

और अधिक जानें

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

The ReplacementOptions प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | निर्दिष्ट प्रतिस्थापन पाठ के साथ ReplacementOptions का एक नया उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | रंगीन आयत को विकल्प के रूप में लेकर ReplacementOptions वर्ग का एक नया उदाहरण प्रारंभ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | प्रतिस्थापन कार्रवाई: बॉक्स बनाएं या पाठ को बदलें। |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | `ReplacementType.draw_box` विकल्प के लिए रंग (अन्यथा अनदेखा किया जाता है)। |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | कस्टम रेडैक्शन हैंडलर जो उपयोगकर्ताओं को अपनी स्वयं की रेडैक्शन लॉजिक परिभाषित करने की अनुमति देता है। |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की सरणी। |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | पाठ्य प्रतिस्थापन मान। |

### उदाहरण

```python
from groupdocs.redaction.redactions import ReplacementOptions

# मिलते हुए पाठ को प्लेसहोल्डर "[X]" से बदलें
repl_opt = ReplacementOptions("[X]")
```

### Guides
`ReplacementOptions` का उपयोग करने वाले टास्क गाइड्स:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
