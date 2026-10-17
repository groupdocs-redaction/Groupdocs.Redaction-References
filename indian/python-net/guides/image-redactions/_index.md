---
title: "छवि रेडैक्शन"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दिखाता है कि विभिन्न फ़ॉर्मैट जैसे JPG, PNG, TIFF आदि की छवियों से संवेदनशील प्रकृति के डेटा को कैसे रेडैक्ट किया जाए।"
type: docs
url: /hi/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions विभिन्न फ़ॉर्मैट जैसे JPG, PNG, TIFF आदि की छवियों से संवेदनशील प्रकृति के डेटा को रेडैक्ट करने के लिए फीचर्स का सेट प्रदान करता है। पूर्ण सूची के लिए देखें [supported document formats]() लेख।

GroupDocs.Redaction छवियों को रेडैक्ट करने के दो तरीके समर्थन करता है, दोनों अलग-अलग इमेज फ़ाइलों में और एम्बेडेड इमेज में:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction for Python via .NET आपको इमेज मेटाडेटा बदलने की भी अनुमति देता है (जैसे इमेज का EXIF डेटा संपादित करना या "EXIF eraser" के रूप में कार्य करना)।

## Redact image area

इमेज एरिया को रेडैक्ट करने के लिए, आपको [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) क्लास का उपयोग करना होगा:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # रेडैक्ट करने वाले क्षेत्र की ऊपर-बाएँ स्थिति निर्धारित करें
    sample_point = Point(385, 485)
    # रेडैक्ट किए जाने वाले क्षेत्र का आकार निर्धारित करें
    sample_size = Size(1793, 2069)
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.jpg") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # डिफ़ॉल्ट रूप से, रेडैक्टेड दस्तावेज़ PDF फ़ॉर्मेट में सहेजा जाता है
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` इस उदाहरण में उपयोग की गई सैंपल फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) पर क्लिक करें।

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

यदि इस प्रकार की फ़ाइलों पर रेडैक्शन लागू नहीं किया जा सकता, जैसे एम्बेडेड इमेज के बिना MS Word दस्तावेज़, तो [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) होगा।

## Clean image metadata

निम्न उदाहरण दिखाता है कि फोटो या किसी अन्य इमेज से EXIF डेटा (उन्हें मिटाना) कैसे संपादित किया जाए:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # सभी इमेज मेटाडेटा (जैसे EXIF) हटाने के लिए रेडैक्शन विकल्प निर्दिष्ट करें
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # रेडैक्ट की जाने वाली इमेज लोड करें
    with Redactor("./sample.jpg") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(er_opt)

        # रिडैक्ट की गई छवि को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` इस उदाहरण में उपयोग की गई सैंपल फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) पर क्लिक करें।

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

यदि इस प्रकार की फ़ाइलों पर रेडैक्शन लागू नहीं किया जा सकता, जैसे BMP इमेज, तो [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) होगा।

## Redact embedded images

आप दस्तावेज़ के भीतर सभी प्रकार की एम्बेडेड इमेज में इमेज एरिया को रेडैक्ट कर सकते हैं।

निम्न उदाहरण दिखाता है कि Microsoft Word दस्तावेज़ के भीतर सभी एम्बेडेड इमेज को कैसे रेडैक्ट किया जाए:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # रेडैक्ट करने वाले क्षेत्र की ऊपर-बाएँ स्थिति निर्धारित करें
    sample_point = Point(516, 311)
    # रेडैक्ट किए जाने वाले क्षेत्र का आकार निर्धारित करें
    sample_size = Size(170, 35)
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # सभी एम्बेडेड इमेज पर रेडैक्शन लागू करें
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # डिफ़ॉल्ट रूप से, रेडैक्टेड दस्तावेज़ PDF फ़ॉर्मेट में सहेजा जाता है
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` इस उदाहरण में उपयोग की गई सैंपल फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) पर क्लिक करें।

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

यदि इस प्रकार की फ़ाइलों पर रेडैक्शन लागू नहीं किया जा सकता, जैसे स्प्रेडशीट दस्तावेज़, तो [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) होगा।

## Multi-frame images

आप एक मल्टी-फ़्रेम इमेज से दिए गए मूल और फ़्रेम संख्या के साथ फ़्रेम हटा सकते हैं। अतिरिक्त जानकारी के लिए देखें [remove page redactions]() लेख।

कुछ इमेज फ़ॉर्मैट, जैसे DjVu दस्तावेज़, को [pre-rasterization]() की आवश्यकता होती है और आगे PDF फ़ॉर्मैट में सहेजना पड़ता है।
