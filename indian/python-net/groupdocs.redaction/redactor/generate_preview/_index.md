---
title: "generate_preview मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "निर्दिष्ट छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियों को उत्पन्न करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactor/generate_preview/
is_root: false
weight: 1050
---


## generate_preview {#preview_options}

निर्दिष्ट छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियों को उत्पन्न करता है।

प्रिव्यू `preview_options` में परिभाषित सेटिंग्स के अनुसार उत्पन्न किया जाता है, जिसमें इमेज फ़ॉर्मेट, आयाम, पेज रेंज, और पेज स्ट्रीम बनाने व रिलीज़ करने के लिए कॉलबैक्स शामिल हैं।

```python
def generate_preview(self, preview_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| preview_options | `PreviewOptions` | छवि गुण और पृष्ठ सीमा सेटिंग्स। |

### उदाहरण

```python
from groupdocs.redaction import Redactor, PreviewOptions, PreviewFormats

def create_page_stream(page_number):
    # दिए गए पेज की प्रिव्यू इमेज के लिए एक लिखने योग्य फ़ाइल स्ट्रीम लौटाता है।
    path = f"C:/Temp/page_{page_number}.png"
    return open(path, "wb")

def release_page_stream(page_number, page_stream):
    # प्रिव्यू इमेज लिखे जाने के बाद कॉल किया जाता है।
    page_stream.close()

preview_options = PreviewOptions(
    create_page_stream=create_page_stream,
    release_page_stream=release_page_stream,
)
preview_options.preview_format = PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("C:/Temp/SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### संबंधित देखें
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
