---
title: ExactPhraseRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a text redaction that replaces an exact phrase in the document's text, case insensitive by default."
type: docs
url: /python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

Represents a text redaction that replaces an exact phrase in the document's text, case insensitive by default.

Learn more
- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/python-net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/python-net/text-redactions/)

The ExactPhraseRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initializes a new instance of ExactPhraseRedaction class in case insensitive mode. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initializes a new ExactPhraseRedaction. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | The description of the redaction, containing its name and parameters. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | The property indicates whether the search is case-sensitive. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | The text direction flag indicating whether the text is right-to-left; defaults to False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | The string to search and replace. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | The [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) instance specifying the type of text replacement. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | The OCR connector implementation used to extract text from graphic content. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # Case-sensitive phrase replacement
    redactor.apply(ExactPhraseRedaction("Emily Johnson", True, ReplacementOptions("[personal]")))
    # Case-insensitive phrase replacement (default)
    redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Task guides that use `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Quick Start Guide](/redaction/python-net/guides/quick-start-guide/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Use redaction callback](/redaction/python-net/guides/use-redaction-callback/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Load with file type](/redaction/python-net/guides/load-with-file-type/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)
* [Save Word with OOXML compliance](/redaction/python-net/guides/save-word-with-ooxml-compliance/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
