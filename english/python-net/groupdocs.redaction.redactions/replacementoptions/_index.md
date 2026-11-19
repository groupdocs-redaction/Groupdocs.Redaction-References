---
title: ReplacementOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents options for matched text replacement."
type: docs
url: /python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

Represents options for matched text replacement.

Learn more:

- More details about document text redactions: <https://docs.groupdocs.com/redaction/python-net/text-redactions/>
- More details about redaction filters: <https://docs.groupdocs.com/redaction/python-net/use-pdf-redaction-filters/>

The ReplacementOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | Initializes a new instance of ReplacementOptions with the specified replacement text. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | Initializes a new instance of ReplacementOptions class with a colored rectangle as an option. |

### Properties
| Property | Description |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | The replacement action: draw box or replace text. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | The color used for a `ReplacementType.draw_box` option (ignored otherwise). |
| [box_fill_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_fill_color/) | The color used for a draw box replacement. This property is obsolete; use [`ReplacementOptions.box_color`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) instead. |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | The custom redaction [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) handler that allows users to define their own redaction logic. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | The array of filters to apply with this redaction. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | The textual replacement value. |

### Example

```python
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.redaction import Redactor

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    redactor.save()
```

### Guides
Task guides that use `ReplacementOptions`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Quick Start Guide](/redaction/python-net/guides/quick-start-guide/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Use redaction callback](/redaction/python-net/guides/use-redaction-callback/)
* [Use PageAreaRedaction](/redaction/python-net/guides/use-page-area-redaction/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Load with file type](/redaction/python-net/guides/load-with-file-type/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)
* [Save Word with OOXML compliance](/redaction/python-net/guides/save-word-with-ooxml-compliance/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
