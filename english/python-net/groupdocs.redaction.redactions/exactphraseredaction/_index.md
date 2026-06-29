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

Learn more:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

The ExactPhraseRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | Initializes a new instance of ExactPhraseRedaction in case‑insensitive mode. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | Initializes a new ExactPhraseRedaction instance. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | The description of the redaction, containing the redaction name and parameters. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | The value indicating whether the search is case-sensitive. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | The text direction flag indicating whether the text is right‑to‑left. Defaults to False. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | The string to search and replace. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | The [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) instance specifying the type of text replacement. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | The IOcrConnector implementation used to extract text from graphic content. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # case‑sensitive replacement
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
Task guides that use `ExactPhraseRedaction`:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
