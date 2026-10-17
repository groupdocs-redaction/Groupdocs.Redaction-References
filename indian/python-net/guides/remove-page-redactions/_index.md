---
title: "पृष्ठ रिडैक्शन हटाएँ"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दर्शाता है कि कैसे संवेदनशील डेटा वाले पृष्ठों को आपके PDF, प्रस्तुति और स्प्रेडशीट दस्तावेज़ों से हटाया जाए।"
type: docs
url: /hi/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction आपको PDF दस्तावेज़ों से पृष्ठ, प्रस्तुतियों से स्लाइड और स्प्रेडशीट दस्तावेज़ों से वर्कशीट आसानी से हटाने की सुविधा देता है।

GroupDocs.Redaction API के साथ आप पृष्ठ सीमा को उसके सापेक्ष स्थान (शुरुआत या अंत), शून्य-आधारित सूचकांक और हटाए जाने वाले पृष्ठों की संख्या के माध्यम से निर्दिष्ट करके पृष्ठ हटा सकते हैं। वर्तमान में समर्थित फ़ॉर्मेट हैं: PDF, प्रस्तुतियाँ (Microsoft PowerPoint, OpenOffice Presentations), वर्ड प्रोसेसिंग दस्तावेज़ (Microsoft Word, OpenOffice Texts, Rich Text Files), स्प्रेडशीट (Microsoft Excel, OpenOffice Spreadsheets, आदि) और मल्टी‑फ़्रेम छवियाँ।

## Remove page range

नीचे के उदाहरण में, हम दस्तावेज़ से 2रा, 3रा और 4था पृष्ठ हटाते हैं, यदि दस्तावेज़ में पर्याप्त पृष्ठ हों।

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./multipage_sample.pdf") as redactor:
        # दस्तावेज़ जानकारी प्राप्त करें
        doc_info = redactor.get_document_info()

        # कम से कम 4 पृष्ठ आवश्यक हैं
        if doc_info.page_count > 3:
            # 2रे पृष्ठ (शून्य-आधारित सूचकांक 1) से शुरू करके 3 पृष्ठ हटाएँ
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # रेडैक्शन लागू करें
            result = redactor.apply(rem_opt)

            # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) क्लिक करें।

## Remove last page

कुछ मामलों में आपको अंतिम पृष्ठ या कई पृष्ठ हटाने की आवश्यकता हो सकती है, चाहे पृष्ठों की संख्या कुछ भी हो।

निम्नलिखित उदाहरण दर्शाता है कि दस्तावेज़ से अंतिम पृष्ठ कैसे हटाया जाए:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # दस्तावेज़ के अंत से 1 पृष्ठ हटाएँ
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./multipage_sample.pdf") as redactor:
        # दस्तावेज़ जानकारी प्राप्त करें
        doc_info = redactor.get_document_info()

        # कम से कम 2 पृष्ठ आवश्यक हैं ताकि दस्तावेज़ खाली न रहे
        if doc_info.page_count > 1:
            # रेडैक्शन लागू करें
            result = redactor.apply(rem_opt)

            # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) क्लिक करें।

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

यदि मल्टी‑फ़्रेम छवि है तो आपको कई फ्रेम (जिन्हें "पृष्ठ" माना जाता है) हटाने की आवश्यकता हो सकती है।

निम्नलिखित उदाहरण दर्शाता है कि एनिमेटेड GIF छवि से 3 फ्रेम कैसे हटाए जाएँ:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # 3रे फ्रेम (शून्य-आधारित सूचकांक 2) से शुरू करके फ्रेम हटाएँ
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # रिडैक्ट करने के लिए मल्टी‑फ़्रेम छवि लोड करें
    with Redactor("./sample.gif") as redactor:
        # दस्तावेज़ जानकारी प्राप्त करें
        doc_info = redactor.get_document_info()

        # कम से कम 7 फ्रेम आवश्यक हैं
        if doc_info.page_count >= 7:
            # रेडैक्शन लागू करें
            result = redactor.apply(rem_opt)

            # रिडैक्ट की गई छवि को स्रोत फ़ाइल के बगल में सहेजें
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) क्लिक करें।

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
