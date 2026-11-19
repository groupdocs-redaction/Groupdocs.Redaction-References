---
title: CellColumnRedaction class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a text redaction that replaces text in spreadsheet documents (CSV, Excel, etc.)."
type: docs
url: /python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Represents a text redaction that replaces text in spreadsheet documents (CSV, Excel, etc.).

Learn more
- More details about applying redactions: https://docs.groupdocs.com/redaction/python-net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/python-net/spreadsheet-redactions/

The CellColumnRedaction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Initializes a new CellColumnRedaction. |

### Methods
| Method | Description |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Applies the redaction to a given format instance. |

### Properties
| Property | Description |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | The description of the redaction, containing the redaction name and parameters. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | The column and worksheet filter. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | The regular expression to match. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | The [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) instance specifying the type of text replacement. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | The OCR connector implementation used to extract text from graphic content. (inherited from [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.redactions import CellFilter

with Redactor("sales.xlsx") as redactor:
    filter = CellFilter()
    filter.column_index = 1  # zero-based second column
    filter.work_sheet_name = "Customers"

    expression = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    change_log = redactor.apply(
        CellColumnRedaction(filter, expression, ReplacementOptions("[customer email]"))
    )
    # Optionally inspect change_log.status
    redactor.save()
```

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
