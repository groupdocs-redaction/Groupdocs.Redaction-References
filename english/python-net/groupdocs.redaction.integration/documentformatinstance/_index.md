---
title: DocumentFormatInstance class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a specific format of a document."
type: docs
url: /python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Represents a specific format of a document. Custom document types are implemented in .NET;

from Python, a format handler is reached through [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/).

The DocumentFormatInstance type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Performs initialization of the instance of document format handler. |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Checks for [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) implementation and invokes it, if specified. |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Loads the document from a stream. |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Checks if the given stream contains a document supported by this format instance. |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Saves the document to a stream. |

### Properties
| Property | Description |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | The password for password-protected documents. |

### Example

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Open .dump files with the plain-text format handler
config = RedactorConfiguration.get_instance()
text_format = config.find_format(".txt")  # a DocumentFormatConfiguration
text_format.extension_filter = text_format.extension_filter + ",.dump"
```

### See Also
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
