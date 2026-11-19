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

- [Loading documents](https://docs.groupdocs.com/redaction/python-net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/python-net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/python-net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/python-net/load-password-protected-file/)

The LoadOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | Initializes a new instance of LoadOptions class. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#file_type) | Initializes a new LoadOptions instance with the specified file type. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Initializes a new LoadOptions instance with the specified password. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Initializes a new LoadOptions instance with a pre‑rasterization flag. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Initializes a new LoadOptions instance with an optional password and an optional pre‑rasterization flag. |

### Properties
| Property | Description |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction.options/loadoptions/file_type/) | The type of the file to open. |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | The password for password-protected documents. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | The pre-rasterize flag indicating whether the file should be pre-rasterized. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def load_password_protected_file():
    # Specify the load options with the document password
    load_opt = LoadOptions("mypassword")

    # Specify the redaction options
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("Emily Johnson", repl_opt)

    # Load the password-protected document to be redacted
    with Redactor("./protected.docx", load_opt) as redactor:
        redactor.apply(ex_red)

        # Save the redacted document in its original format
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")

if __name__ == "__main__":
    load_password_protected_file()
```

### Guides
Task guides that use `LoadOptions`:

* [Use redaction callback](/redaction/python-net/guides/use-redaction-callback/)
* [OCR usage basics](/redaction/python-net/guides/ocr-usage-basics/)
* [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/)
* [Load with file type](/redaction/python-net/guides/load-with-file-type/)
* [Use advanced logging](/redaction/python-net/guides/use-advanced-logging/)

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
