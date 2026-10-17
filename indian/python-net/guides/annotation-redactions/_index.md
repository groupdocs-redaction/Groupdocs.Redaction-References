---
title: "एनोटेशन रेडैक्शन"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख विभिन्न फ़ॉर्मेट्स जैसे PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX और अन्य दस्तावेज़ों के लिए एनोटेशन रेडैक्शन के कार्यान्वयन को दर्शाता है।"
type: docs
url: /hi/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


GroupDocs.Redaction API के साथ आप PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX और अन्य विभिन्न फ़ॉर्मेट्स के दस्तावेज़ों के लिए एनोटेशन रेडैक्शन लागू कर सकते हैं। पूर्ण सूची के लिए [supported document formats]() लेख देखें।

GroupDocs.Redactions एक लचीला API प्रदान करता है जो एनोटेशन टेक्स्ट से संवेदनशील डेटा को हटाने या नियमित अभिव्यक्ति द्वारा पूरी तरह से एनोटेशन को हटाने की अनुमति देता है।

## Remove annotations (comments etc)

आप GroupDocs.Redaction का उपयोग करके दस्तावेज़ से सभी या विशिष्ट टिप्पणियों और अन्य एनोटेशन को हटा सकते हैं। उदाहरण के लिए, हम दस्तावेज़ से सभी टिप्पणियों को हटा सकते हैं, जिनके शरीर में "use", "show" या "describe" जैसे शब्द हों:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # पैटर्न से मेल खाने वाले एनोटेशन को हटाने के लिए रेडैक्शन विकल्प निर्दिष्ट करें
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./annotated.xlsx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(a_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) पर क्लिक करें।

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

आप बिना किसी तर्क के कंस्ट्रक्टर का उपयोग करके दस्तावेज़ के भीतर सभी एनोटेशन हटा सकते हैं।

## Redact annotations

सभी या विशिष्ट एनोटेशन को हटाने के बजाय, आप एनोटेशन टेक्स्ट से संवेदनशील डेटा हटा सकते हैं। उदाहरण के लिए, हम दिए गए दस्तावेज़ में "John" के सभी उल्लेखों को हटा सकते हैं, जैसे:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # रेडैक्शन विकल्प निर्दिष्ट करें: खोज पैटर्न और प्रतिस्थापन स्ट्रिंग
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./annotated.xlsx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(a_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) पर क्लिक करें।

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
