---
title: ReleasePageStream class
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Represents a method which releases a stream created by the CreatePageStream delegate."
type: docs
url: /python-net/groupdocs.redaction.options/releasepagestream/
is_root: false
weight: 100
---


## ReleasePageStream class

Represents a method which releases a stream created by the [`CreatePageStream`](/redaction/python-net/groupdocs.redaction.options/createpagestream/) delegate.

The ReleasePageStream type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/releasepagestream/__init__/#object-method) |  |

### Methods
| Method | Description |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke/#page_number-page_stream-callback-object) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/end_invoke/#result) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke/#page_number-page_stream) |  |

### Example

```python
import io
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import PreviewOptions

def create_delegate(page_number):
    return io.BytesIO()

def release_delegate(page_number, page_stream):
    # The engine has written and closed the page: the BytesIO holds the image
    print("page %d: %d bytes" % (page_number, len(page_stream.getvalue())))

preview_options = PreviewOptions(create_delegate, release_delegate)
preview_options.preview_format = PreviewOptions.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor("SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### See Also
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
