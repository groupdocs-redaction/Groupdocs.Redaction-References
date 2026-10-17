---
title: "generate_preview मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "निर्दिष्ट छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियों को उत्पन्न करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/ipreviewable/generate_preview/
is_root: false
weight: 1010
---


## generate_preview {#preview_options}

निर्दिष्ट छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियों को उत्पन्न करता है।

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

with Redactor("document.pdf") as redactor:
    options = PreviewOptions(
        format=PreviewFormats.PNG,
        start_page=1,
        end_page=5,
        create_page_stream=lambda page: open(f"page_{page}.png", "wb")
    )
    redactor.generate_preview(options)
```

### संबंधित देखें
* class [`IPreviewable`](/redaction/python-net/groupdocs.redaction.integration/ipreviewable/)
