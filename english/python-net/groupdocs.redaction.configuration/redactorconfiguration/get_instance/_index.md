---
title: get_instance method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Provides a singleton instance with the default configuration of built-in formats."
type: docs
url: /python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1020
---


## get_instance

Provides a singleton instance with the default configuration of built-in formats.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.configuration import RedactorConfiguration
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Obtain the singleton configuration
config = RedactorConfiguration.get_instance()

# Extend the .txt format to also handle .dump files
txt_settings = config.find_format(".txt")
txt_settings.extension_filter = txt_settings.extension_filter + ",.dump"

# Define redaction options
repl_opt = ReplacementOptions("[redacted]")
ex_red = ExactPhraseRedaction("dolor", repl_opt)

# Load and redact a document with the new extension
with Redactor("./sample.dump") as redactor:
    redactor.apply(ex_red)

    # Save the redacted document
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
```

### See Also
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
