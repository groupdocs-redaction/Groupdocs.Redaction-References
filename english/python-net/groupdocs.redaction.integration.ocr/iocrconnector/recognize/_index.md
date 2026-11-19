---
title: recognize method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Processes OCR for an image provided as a stream."
type: docs
url: /python-net/groupdocs.redaction.integration.ocr/iocrconnector/recognize/
is_root: false
weight: 1010
---


## recognize {#image_stream}

Processes OCR for an image provided as a stream.

```python
def recognize(self, image_stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | Stream containing an image to process. |

**Returns:** RecognizedImage: Structured recognized text containing lines, words and their bounding rectangles.

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.integration.ocr import RecognizedImage, TextFragment, TextLine
from groupdocs.redaction.options import LoadOptions, RedactorSettings
from groupdocs.redaction.options.drawing import Color, Rectangle
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

class MyConnector:
    def recognize(self, image_stream):
        # In a real implementation, hand the bytes to an OCR engine.
        data = image_stream.read()
        # One fragment per line: engine 26.10 paints no phrase that spans two fragments.
        line = TextLine([TextFragment("Emily Johnson", Rectangle(40, 40, 230, 40))])
        return RecognizedImage([line])

with Redactor("scan.png", LoadOptions(), RedactorSettings(ocr_connector=MyConnector())) as redactor:
    result = redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions(Color.black)))
    print(result.status.name)
```

### Aliases

These names call `recognize` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `recognize_stream` | `recognize_stream(image_stream)` |
| `recognize_streams` | `recognize_streams(image_stream)` |

### See Also
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/)
