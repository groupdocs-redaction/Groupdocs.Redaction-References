---
title: IRedactionCallback class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Defines methods required for receiving information on each redaction change and optionally preventing it."
type: docs
url: /python-net/groupdocs.redaction.redactions/iredactioncallback/
is_root: false
weight: 100
---


## IRedactionCallback class

Defines methods required for receiving information on each redaction change and optionally preventing it.

Learn more:

- More details about implementing [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback (https://docs.groupdocs.com/redaction/python-net/use-redaction-callback/)

The IRedactionCallback type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [accept_redaction](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/accept_redaction/#description) | Triggered right before applying any redaction to the document, allowing logging or forbidding it. |

### Example

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, RedactorSettings
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

class RedactionDump(object):
    def accept_redaction(self, description):
        print(
            f"{description.redaction_type} redaction, "
            f"{description.action_type} action, "
            f"item {description.original_text}. ",
            end=''
        )
        if description.replacement is not None:
            print(
                f"Text {description.replacement.original_text} is replaced with "
                f"{description.replacement.replacement}. ",
                end=''
            )
        print()
        # Return False to prevent this change during the redaction process
        return True

# Pass an instance to RedactorSettings, the third Redactor argument
with Redactor("sample.docx", LoadOptions(), RedactorSettings(RedactionDump())) as redactor:
    redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions("[personal]")))
    redactor.save()
```

### See Also
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
