---
title: OCR usage basics
linkTitle: "OCR usage basics"
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Write an OCR connector for GroupDocs.Redaction for Python via .NET: what it receives, what it returns, and how the engine redacts the recognized text."
type: docs
url: /python-net/guides/ocr-usage-basics/
is_root: false
weight: 160
---


An OCR connector is an object with a `recognize(image_stream)` method, or a function that takes `image_stream`:

* `image_stream` is the image to recognize, valid during the call. `image_stream.read()` gives its bytes.
* It returns a [RecognizedImage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/), or `None` for an image with no text.

A [`RecognizedImage`](/redaction/python-net/groupdocs.redaction.integration.ocr/recognizedimage/) holds the lines of text, each a [TextLine](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.integration.ocr/textline/) of [TextFragment](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.integration.ocr/textfragment/) objects. A fragment is a piece of text with the rectangle, in pixels from the image's top-left corner, where it was found. Report each line as one fragment: its text and the rectangle that covers it.

GroupDocs.Redaction searches the recognized text for the redaction's phrase or expression. It covers a match inside a fragment, placing the box by the match's position in the fragment's text. A match that spans two fragments is reported `APPLIED` but not covered (GroupDocs.Redaction 26.10), which is why a line is one fragment. An exception the connector raises reaches the caller of `apply()`.

## A connector without an OCR engine

The connector below stands in for an OCR engine: for every image, it reports the line "Customer: Emily Johnson" where it is in the sample scan. It shows the shapes a real connector returns, and it runs without any OCR software:

{{< tabs "code-example-ocr-usage-basics" >}}
{{< tab "ocr_usage_basics.py" >}}
```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.integration.ocr import RecognizedImage, TextFragment, TextLine
from groupdocs.redaction.options import LoadOptions, RedactorSettings, SaveOptions
from groupdocs.redaction.options.drawing import Color, Rectangle
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

class FixedResultOcrConnector(object):
    """Reports the line "Customer: Emily Johnson" at the same place in every image."""

    def __init__(self):
        self.images = 0

    def recognize(self, image_stream):
        self.images += 1
        image_bytes = image_stream.read()  # what a real OCR engine would read
        # One fragment per line: its text and the rectangle that covers it, in pixels
        line = TextLine([TextFragment("Customer: Emily Johnson", Rectangle(122, 365, 338, 28))])
        return RecognizedImage([line])

def ocr_usage_basics():
    connector = FixedResultOcrConnector()
    with Redactor("./scan.png", LoadOptions(), RedactorSettings(connector)) as redactor:
        result = redactor.apply(ExactPhraseRedaction("Emily Johnson", ReplacementOptions(Color.black)))
        print("Images recognized: %d, status: %s" % (connector.images, result.status.name))

        options = SaveOptions()
        options.add_suffix = True
        options.rasterize_to_pdf = False  # keep the PNG format
        result_path = redactor.save(options)
        print("Output saved to " + result_path)

if __name__ == "__main__":
    ocr_usage_basics()
```
{{< /tab >}}
{{< tab "scan.png" >}}

`scan.png` is the sample file used in this example. Click [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/using-ocr/ocr-usage-basics/scan.png) to download it.

{{< /tab >}}
{{< tab "scan_Redacted.png" >}}  
```text
Binary file (PNG, 85 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/using-ocr/ocr-usage-basics/ocr_usage_basics/scan_Redacted.png)
{{< /tab >}}
{{< /tabs >}}

`RedactorSettings(connector)` takes the connector as its only argument. Next to a logger and a redaction callback, pass it by name: `RedactorSettings(logger, callback, connector)` or `RedactorSettings(ocr_connector=connector)`.

For a connector built on a real OCR engine, see [Use Tesseract OCR](/redaction/python-net/guides/use-tesseract-ocr/).
