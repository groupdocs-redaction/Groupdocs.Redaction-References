---
title: "CreatePageStream क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक मेथड को दर्शाता है जो पेज प्रीव्यू डेटा लिखने के लिए स्ट्रीम लौटाता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/createpagestream/
is_root: false
weight: 20
---


## CreatePageStream class

एक मेथड को दर्शाता है जो पेज प्रीव्यू डेटा लिखने के लिए स्ट्रीम लौटाता है।

CreatePageStream प्रकार निम्नलिखित सदस्य उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/createpagestream/__init__/#object-method) |  |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke/#page_number-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/begin_invoke_int32/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/createpagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke/#page_number) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/createpagestream/invoke_int32/) |  |

### उदाहरण

```python
import os
import io
from groupdocs.redaction import Redactor, PreviewOptions

def create_page_stream(page_number: int) -> io.RawIOBase:
    page_path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(page_path, "wb")

preview_options = PreviewOptions(create_page_stream)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
