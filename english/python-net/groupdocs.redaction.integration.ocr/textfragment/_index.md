---
title: TextFragment class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a part of recognized text (word, symbol, etc), extracted by an OCR engine."
type: docs
url: /python-net/groupdocs.redaction.integration.ocr/textfragment/
is_root: false
weight: 30
---


## TextFragment class

Represents a part of recognized text (word, symbol, etc), extracted by an OCR engine.

Learn more:
- More details about using OCR in GroupDocs.Redaction: https://docs.groupdocs.com/redaction/python-net/ocr-usage-basics/

The TextFragment type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/__init__/#text-rectangle) | Initializes a recognized text fragment. |

### Methods
| Method | Description |
| :- | :- |
| [to_string](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/to_string/) | Returns textual content of the recognized text fragment. |

### Properties
| Property | Description |
| :- | :- |
| [bounding_rectangle](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/bounding_rectangle/) | The bounding rectangle of the recognized text fragment; this property is obsolete, use [`TextFragment.rectangle`](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/rectangle/) instead. |
| [rectangle](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/rectangle/) | The bounding rectangle of the recognized text fragment. |
| [text](/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/text/) | The textual content of the recognized text fragment. |

### Example

```python
from groupdocs.redaction.integration.ocr import TextFragment
from groupdocs.redaction.options.drawing import Rectangle

fragment = TextFragment("Emily Johnson", Rectangle(40, 40, 230, 40))
```

### Guides
Task guides that use `TextFragment`:

* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)

### See Also
* module [`groupdocs.redaction.integration.ocr`](/redaction/python-net/groupdocs.redaction.integration.ocr/)
