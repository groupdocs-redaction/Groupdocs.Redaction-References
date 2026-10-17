---
title: "PreviewOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "प्रीव्यू जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट्स सेट करने के विकल्प प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/previewoptions/
is_root: false
weight: 70
---


## PreviewOptions class

प्रीव्यू जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट्स सेट करने के विकल्प प्रदान करता है।

यह क्लास पूर्वावलोकन प्रारूप, छवि आयाम, पृष्ठ संख्याएँ, और प्रत्येक उत्पन्न पृष्ठ के लिए स्ट्रीम बनाने और वैकल्पिक रूप से रिलीज़ करने वाले डेलीगेट्स को निर्दिष्ट करने की अनुमति देती है।

यह PreviewOptions प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream) | एक नया PreviewOptions इंस्टेंस प्रारंभ करता है। आउटपुट स्ट्रीम उपयोग के बाद बंद कर दी जाएगी। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/previewoptions/__init__/#create_page_stream-release_page_stream) | एक नया PreviewOptions इंस्टेंस प्रारंभ करता है, जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस कर दी जाती है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [create_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/create_page_stream/) | पृष्ठ स्ट्रीम निर्माण डेलीगेट। |
| [height](/redaction/python-net/groupdocs.redaction.options/previewoptions/height/) | पृष्ठ प्रीव्यू की ऊँचाई। |
| [page_numbers](/redaction/python-net/groupdocs.redaction.options/previewoptions/page_numbers/) | प्रीव्यू उत्पन्न करने के लिए पृष्ठ संख्याएँ। |
| [preview_format](/redaction/python-net/groupdocs.redaction.options/previewoptions/preview_format/) | प्रीव्यू छवि प्रारूप। |
| [release_page_stream](/redaction/python-net/groupdocs.redaction.options/previewoptions/release_page_stream/) | पृष्ठ प्रीव्यू पूर्णता डेलीगेट। |
| [width](/redaction/python-net/groupdocs.redaction.options/previewoptions/width/) | पृष्ठ प्रीव्यू की चौड़ाई। |

### उदाहरण

```python
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int):
    # दिए गए पृष्ठ की प्रीव्यू छवि के लिए एक फ़ाइल बनाएं
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")  # returns a writable binary stream

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
