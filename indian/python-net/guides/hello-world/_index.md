---
title: "हैलो, वर्ल्ड!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "GroupDocs.Redaction for Python via .NET के साथ जल्दी शुरू करें, एक सरल उदाहरण बनाकर और चलाकर।"
type: docs
url: /hi/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
"Hello, World!" उदाहरण अक्सर GroupDocs.Redaction for Python via .NET का अन्वेषण करते समय पहला कदम होता है। यह एक सरल परीक्षण के रूप में कार्य करता है ताकि यह पुष्टि की जा सके कि आपका विकास वातावरण सही ढंग से सेट है और लाइब्रेरी अपेक्षित रूप से कार्य कर रही है।

## Overview
GroupDocs.Redaction for Python via .NET आपको विभिन्न दस्तावेज़ फ़ॉर्मेट्स से संवेदनशील जानकारी खोजने, रेडैक्ट करने और हटाने की अनुमति देता है। विस्तृत [supported formats](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) इसे विभिन्न उपयोग मामलों के लिए बहुमुखी बनाती है।

## How to redact a document
निम्नलिखित चरण दर्शाते हैं कि GroupDocs.Redaction for Python via .NET का उपयोग करके दस्तावेज़ से संवेदनशील जानकारी को कैसे रेडैक्ट किया जाए:

1. आवश्यक `groupdocs.redaction` क्लासेस आयात करें।
2. रेडैक्शन का वर्णन करें (यहाँ, एक सटीक वाक्यांश जिसे रंगीन बॉक्स से बदलना है)।
3. नमूना दस्तावेज़ के पथ के साथ एक [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) बनाएं।
4. रेडैक्शन लागू करें।
5. परिणाम सहेजें।

## Complete example
नीचे दिया गया उदाहरण "John Doe" वाक्यांश की प्रत्येक घटना को अर्ध-पारदर्शी लाल बॉक्स से बदलता है और रेडैक्टेड दस्तावेज़ को सहेजता है:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # "John Doe" की प्रत्येक घटना पर अर्ध-पारदर्शी लाल बॉक्स बनाएं
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # दस्तावेज़ लोड करें, रेडैक्शन लागू करें, और परिणाम सहेजें
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) पर क्लिक करें।

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

यह उदाहरण परिणाम को `sample_redacted.pdf` नामक PDF में रास्टर करता है, इसलिए रेडैक्टेड सामग्री को पुनः प्राप्त नहीं किया जा सकता (`save()` डिफ़ॉल्ट रूप से PDF में रास्टर करता है; `redacted_file_suffix` विकल्प केवल आउटपुट नाम नियंत्रित करता है)। मूल फ़ॉर्मेट को बनाए रखने के लिए, `rasterize_to_pdf = False` सेट करें।

## Additional resources
यह डेमो GroupDocs.Redaction for Python via .NET के [code samples](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) को संदर्भित करता है।
