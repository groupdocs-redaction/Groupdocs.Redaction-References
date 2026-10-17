---
title: "ReleasePageStream klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Stelt een methode voor die een door de CreatePageStream-delegate gemaakte stream vrijmaakt."
type: docs
url: /nl/python-net/groupdocs.redaction.options/releasepagestream/
is_root: false
weight: 100
---


## ReleasePageStream class

Stelt een methode voor die een stream vrijgeeft die is aangemaakt door de [`CreatePageStream`](/redaction/python-net/groupdocs.redaction.options/createpagestream/) delegate.

Het type ReleasePageStream bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/releasepagestream/__init__/#object-method) |  |

### Methoden
| Methode | Beschrijving |
| :- | :- |
| [begin_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke/#page_number-page_stream-callback-object) |  |
| [begin_invoke_int32](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_int32/) |  |
| [begin_invoke_stream](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_stream/) |  |
| [begin_invoke_streams](/redaction/python-net/groupdocs.redaction.options/releasepagestream/begin_invoke_streams/) |  |
| [end_invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/end_invoke/#result) |  |
| [end_invoke_iasync_result](/redaction/python-net/groupdocs.redaction.options/releasepagestream/end_invoke_iasync_result/) |  |
| [invoke](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke/#page_number-page_stream) |  |
| [invoke_int32](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_int32/) |  |
| [invoke_stream](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_stream/) |  |
| [invoke_streams](/redaction/python-net/groupdocs.redaction.options/releasepagestream/invoke_streams/) |  |

### Voorbeeld

```python
import os
import io
from GroupDocs.Redaction import Redactor
from GroupDocs.Redaction.Options import PreviewOptions

def create_delegate(page_number: int) -> io.RawIOBase:
    path = os.path.join(r"C:\Temp", f"page_{page_number}.png")
    return open(path, "wb")

def release_delegate(page_number: int, page_stream: io.RawIOBase) -> None:
    # Verwerk de stream indien nodig
    page_stream.close()

preview_options = PreviewOptions(create_delegate, release_delegate)
preview_options.preview_format = preview_options.PreviewFormats.PNG
preview_options.height = 640
preview_options.width = 480
preview_options.page_numbers = [1]

with Redactor(r"C:\Temp\SourceFile.pdf") as redactor:
    redactor.generate_preview(preview_options)
```

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
