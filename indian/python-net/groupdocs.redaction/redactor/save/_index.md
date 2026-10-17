---
title: "save मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "दस्तावेज़ को फ़ाइल में निम्नलिखित विकल्पों के साथ सहेजता है: AddSuffix = True, RasterizeToPDF = True।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactor/save/
is_root: false
weight: 1080
---


## save

दस्तावेज़ को फ़ाइल में निम्नलिखित विकल्पों के साथ सहेजता है: AddSuffix = True, RasterizeToPDF = True।

```python
def save(self):
    ...
```

**Returns:** str: Path to redacted document.

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("document.docx") as redactor:
    redactor.apply(ExactPhraseRedaction("secret", ReplacementOptions("[X]")))
    options = SaveOptions()
    options.add_suffix = True
    options.rasterize_to_pdf = True
    result_path = redactor.save(options)
    print(f"Saved to {result_path}")
```

## save {#save_options}

दस्तावेज़ को फ़ाइल में सहेजता है।

```python
def save(self, save_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| save_options | `SaveOptions` | सफ़िक्स जोड़ने या रास्टराइज़ करने के विकल्प। |

**Returns:** Path to redacted document.

### उदाहरण

```python
from datetime import datetime
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions


def save_in_original_format():
    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        redactor.apply(ex_red)

        # रेडैक्टेड दस्तावेज़ को उसकी मूल फ़ॉर्मेट में तिथि सफ़िक्स के साथ सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = datetime.now().strftime("%Y-%m-%d %H-%M-%S")

        result_path = redactor.save(so)
        print(f"Document redacted successfully.\nCheck output in {result_path}.")


if __name__ == "__main__":
    save_in_original_format()
```

## save {#document-rasterization_options}

कस्टम स्थान सहित दस्तावेज़ को स्ट्रीम में सहेजता है।

```python
def save(self, document, rasterization_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| document | `io.RawIOBase` | लक्ष्य स्ट्रीम। |
| rasterization_options | `RasterizationOptions` | रास्टराइज़ करने या न करने और रास्टराइज़ेशन के लिए पृष्ठ निर्दिष्ट करने के विकल्प। |

### उदाहरण

```python
import io
from groupdocs.redaction.options import RasterizationOptions
from groupdocs.redaction import Redactor

with Redactor("document.pptx") as redactor:
    # केवल पहले स्लाइड को प्रोसेस करने के लिए रास्टराइज़ेशन कॉन्फ़िगर करें
    ro = RasterizationOptions()
    ro.page_index = 0
    ro.page_count = 1

    stream = io.BytesIO()
    redactor.save(stream, ro)

    # अब BytesIO ऑब्जेक्ट में सहेजा गया दस्तावेज़ शामिल है
    data = stream.getvalue()
```

### संबंधित देखें
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
