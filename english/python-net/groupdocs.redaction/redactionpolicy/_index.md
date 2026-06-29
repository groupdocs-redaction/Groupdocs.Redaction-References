---
title: RedactionPolicy class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a sanitization policy, containing a set of specific redactions to apply."
type: docs
url: /python-net/groupdocs.redaction/redactionpolicy/
is_root: false
weight: 120
---


## RedactionPolicy class

Represents a sanitization policy, containing a set of specific redactions to apply.

**Learn more**
- More details about policies: https://docs.groupdocs.com/redaction/net/use-redaction-policies/
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/

The RedactionPolicy type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/) | Initializes a new RedactionPolicy instance. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactionpolicy/__init__/#redactions) | Initializes a new RedactionPolicy with a specific list of redactions. |

### Methods
| Method | Description |
| :- | :- |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#file_path) | Loads a RedactionPolicy from an XML file. |
| [load](/redaction/python-net/groupdocs.redaction/redactionpolicy/load/#input) | Loads a RedactionPolicy instance from a stream containing XML configuration. |
| [load_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_file/) |  |
| [load_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_streams/) |  |
| [load_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/load_string/) |  |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#file_path) | Saves the redaction policy to a file. |
| [save](/redaction/python-net/groupdocs.redaction/redactionpolicy/save/#output) | Saves the redaction policy to a stream. |
| [save_file](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_file/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_streams/) |  |
| [save_string](/redaction/python-net/groupdocs.redaction/redactionpolicy/save_string/) |  |

### Properties
| Property | Description |
| :- | :- |
| [redactions](/redaction/python-net/groupdocs.redaction/redactionpolicy/redactions/) | The list of fully configured [`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)-derived classes. |

### Example

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

# Build a reusable policy in memory
policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])

# Apply the policy to a document
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Guides
Task guides that use `RedactionPolicy`:

* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### See Also
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
