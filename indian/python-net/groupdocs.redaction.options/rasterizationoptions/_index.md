---
title: "RasterizationOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "फ़ाइलों को PDF में कनवर्ट करने के विकल्प प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

फ़ाइलों को PDF में कनवर्ट करने के विकल्प प्रदान करता है।

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

RasterizationOptions प्रकार निम्नलिखित सदस्य उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | एक नया उदाहरण प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत करता है। |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | लागू करने के लिए एक उन्नत रास्टराइज़ेशन विकल्प पंजीकृत करता है। |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | PDF अनुपालन स्तर। |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | सक्षम फ़्लैग दर्शाता है कि क्या दस्तावेज़ के सभी पृष्ठों को छवियों में परिवर्तित किया जाता है और एकल PDF फ़ाइल में रखा जाता है। डिफ़ॉल्ट रूप से True; रास्टराइज़ेशन से बचने के लिए इसे False सेट करें। |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | यदि उन्नत रास्टराइज़ेशन विकल्प सेट हैं तो संकेतक True होता है। |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | PDF में परिवर्तित किए जाने वाले पृष्ठों की संख्या। |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | PDF में परिवर्तित करने के लिए पहले पृष्ठ (0-आधारित) का सूचकांक। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
