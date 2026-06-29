---
title: LoadOptions class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides options that will be used to open a file."
type: docs
url: /python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Provides options that will be used to open a file.

Learn more
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

The LoadOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initializes a new instance of LoadOptions class. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initializes a new instance of LoadOptions with the specified password. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initializes a new LoadOptions instance with the specified pre‑rasterization flag. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initializes a new LoadOptions instance with the specified password. |

### Properties
| Property | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | The password for password-protected documents. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | The pre_rasterize flag indicating whether the file should be pre‑rasterized. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Specify the load options with the document password
load_opt = LoadOptions("mypassword")

# Define a redaction
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Open the password‑protected document
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Save the redacted document
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
