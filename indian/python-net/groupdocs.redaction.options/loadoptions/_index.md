---
title: "LoadOptions क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

फ़ाइल खोलने के लिए उपयोग किए जाने वाले विकल्प प्रदान करता है।

और अधिक जानें
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

LoadOptions प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | LoadOptions क्लास का नया उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | निर्दिष्ट पासवर्ड के साथ LoadOptions का नया उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | निर्दिष्ट pre‑rasterization फ़्लैग के साथ नया LoadOptions उदाहरण प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | निर्दिष्ट पासवर्ड के साथ नया LoadOptions उदाहरण प्रारंभ करता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | पासवर्ड-संरक्षित दस्तावेज़ों के लिए पासवर्ड। |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | pre_rasterize फ़्लैग यह दर्शाता है कि फ़ाइल को पूर्व‑रास्टराइज़ किया जाना चाहिए या नहीं। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# दस्तावेज़ पासवर्ड के साथ लोड विकल्प निर्दिष्ट करें
load_opt = LoadOptions("mypassword")

# एक रिडैक्शन परिभाषित करें
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# पासवर्ड‑सुरक्षित दस्तावेज़ खोलें
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # रिडैक्टेड दस्तावेज़ सहेजें
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### संबंधित देखें
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
