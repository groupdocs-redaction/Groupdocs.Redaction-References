---
title: RecognizedImage class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents text, extracted from an image as a result of its recognition process."
type: docs
url: /python-net/groupdocs.redaction.integration.ocr/recognizedimage/
is_root: false
weight: 20
---


## RecognizedImage class

Represents text, extracted from an image as a result of its recognition process.

Learn more
- More details about using OCR in GroupDocs.Redaction: https://docs.groupdocs.com/redaction/python-net/ocr-usage-basics/

The RecognizedImage type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/__init__/#lines) | Initializes a new instance of the class using a set of recognized lines. |

### Methods
| Method | Description |
| :- | :- |
| [to_string](/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/to_string/) | Returns the textual equivalent of the structured text. |

### Properties
| Property | Description |
| :- | :- |
| [lines](/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/lines/) | The lines of text, with their fragments, recognized within the document. |
| [text](/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/text/) | The textual equivalent of the structured text. |

### Example

```python
from groupdocs.redaction.integration.ocr import RecognizedImage, TextLine, TextFragment
from groupdocs.redaction.options.drawing import Rectangle

recognized = RecognizedImage([
    TextLine([TextFragment("Emily Johnson", Rectangle(40, 40, 230, 40))])
])
```

### Guides
Task guides that use `RecognizedImage`:

* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)

### See Also
* module [`groupdocs.redaction.integration.ocr`](/redaction/python-net/groupdocs.redaction.integration.ocr/)
