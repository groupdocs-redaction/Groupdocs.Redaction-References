---
title: "SaveOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "आउटपुट फ़ाइल नाम बदलने और/या दस्तावेज़ को इमेज‑आधारित PDF (रास्टराइज़ेशन) में बदलने के विकल्प प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

आउटपुट फ़ाइल नाम बदलने और/या दस्तावेज़ को इमेज‑आधारित PDF (रास्टराइज़ेशन) में बदलने के विकल्प प्रदान करता है।

और अधिक जानें:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

SaveOptions प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | डिफ़ॉल्ट सेटिंग्स के साथ एक नया इंस्टेंस प्रारंभ करता है: rasterize_to_pdf फ़ॉल्स है और add_suffix फ़ॉल्स है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | दिए गए पैरामीटरों के साथ एक नया इंस्टेंस प्रारंभ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | add_suffix प्रॉपर्टी दर्शाती है कि फ़ाइल नाम को सहेजने से पहले बदलना चाहिए या नहीं। डिफ़ॉल्ट रूप से फ़ॉल्स है। |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | रास्टराइज़ेशन सेटिंग्स। |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | फ़्लैग जो दर्शाता है कि दस्तावेज़ के सभी पृष्ठ छवियों में परिवर्तित किए गए हैं और एकल PDF फ़ाइल में संयोजित किए गए हैं। |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | आउटपुट फ़ाइल नाम के लिए कस्टम सफ़िक्स। यदि निर्दिष्ट नहीं किया गया, तो [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) स्थिरांक का उपयोग किया जाता है। |

### फ़ील्ड्स
| फ़ील्ड | विवरण |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | डिफ़ॉल्ट सफ़िक्स मान को दर्शाता है, जो "Redacted" है। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # डिफ़ॉल्ट विकल्पों के साथ दस्तावेज़ सहेजें (PDF में रास्टराइज़ करें और सफ़िक्स जोड़ें)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
`SaveOptions` का उपयोग करने वाले टास्क गाइड्स:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
