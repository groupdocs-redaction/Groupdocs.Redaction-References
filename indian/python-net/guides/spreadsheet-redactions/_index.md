---
title: "स्प्रेडशीट रिडैक्शन"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दर्शाता है कि Python रिडैक्शन API कैसे आपके XLS, XLSX, ODS स्प्रेडशीट दस्तावेज़ फ़ॉर्मेट और अन्य से संवेदनशील या निजी प्रकृति के डेटा को रिडैक्ट करने की अनुमति देता है।"
type: docs
url: /hi/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction आपके XLS, XLSX, ODS स्प्रेडशीट दस्तावेज़ फ़ॉर्मेट और अन्य से संवेदनशील या निजी प्रकृति के डेटा को रिडैक्ट करने की अनुमति देता है। पूर्ण सूची के लिए देखें [supported document formats]() लेख।

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # रिडैक्ट करने के लिए स्प्रेडशीट लोड करें
    with Redactor("./sample.xlsx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) पर क्लिक करें।

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
