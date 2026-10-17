---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "डिफ़ॉल्ट सेटिंग्स के साथ एक नया इंस्टेंस प्रारंभ करता है: rasterizetopdf False है और addsuffix False है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/saveoptions/__init__/
is_root: false
weight: 10
---


## __init__

डिफ़ॉल्ट सेटिंग्स के साथ एक नया इंस्टेंस प्रारंभ करता है: rasterize_to_pdf फ़ॉल्स है और add_suffix फ़ॉल्स है।

```python
def __init__(self):
    ...
```

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

with Redactor("./sample.docx") as redactor:
    redactor.apply(ex_red)
    save_options = SaveOptions()  # defaults: rasterize_to_pdf=False, add_suffix=False
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}.")
```

## __init__ {#rasterize_to_pdf-suffix}

दिए गए पैरामीटरों के साथ एक नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, rasterize_to_pdf, suffix):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| rasterize_to_pdf | `bool` | True, यदि दस्तावेज़ में सभी पृष्ठों को छवियों में परिवर्तित करके एक ही PDF फ़ाइल में रखा जाना चाहिए। |
| suffix | `str` | यह टेक्स्ट फ़ाइल नाम के अंत में जोड़ा जाएगा; यदि खाली नहीं है तो `add_suffix` को True सेट भी करता है। |

### उदाहरण

```python
from groupdocs.redaction.options import SaveOptions

# डिफ़ॉल्ट सेटिंग्स के साथ सहेजने के विकल्प बनाएं
options = SaveOptions()
options.add_suffix = True
options.rasterize_to_pdf = True
options.redacted_file_suffix = "redacted"
```

### संबंधित देखें
* class [`SaveOptions`](/redaction/python-net/groupdocs.redaction.options/saveoptions/)
