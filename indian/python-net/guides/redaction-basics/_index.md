---
title: "रेडैक्शन मूलभूत बातें"
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दिखाता है कि Python डेवलपर्स अपने दस्तावेज़ों में मेटाडेटा, इमेज, एनोटेशन और टेक्स्ट रेडैक्शन कैसे लागू कर सकते हैं। विभिन्न प्रकार के दस्तावेज़ फ़ॉर्मैट समर्थित हैं, जैसे PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX और अन्य।"
type: docs
url: /hi/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


GroupDocs.Redaction दस्तावेज़ रेडैक्शन सुविधाओं का प्रभावी सेट समर्थन करता है। यह [text](), [metadata](), [annotations](), [images]() के लिए रेडैक्शन लागू करने की अनुमति देता है।

विभिन्न प्रकार के दस्तावेज़ फ़ॉर्मैट समर्थित हैं, जैसे: PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX और अन्य। पूर्ण समर्थित फ़ॉर्मैट सूची के लिए [supported document formats]() लेख देखें।

## Redaction types

GroupDocs.Redaction निम्नलिखित रेडैक्शन प्रकारों के साथ आता है:

| प्रकार | विवरण | क्लासेस |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

एक दस्तावेज़ पर रेडैक्शन लागू करना [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) मेथड के माध्यम से किया जाता है। परिणामस्वरूप, आपको [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) इंस्टेंस मिलता है, जिसमें प्रत्येक लागू किए गए रेडैक्शन के लिए एक लॉग एंट्री होती है। एंट्री में [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) इंस्टेंस का संदर्भ शामिल होता है, जिसमें उसके विकल्प, ऑपरेशन की स्थिति (नीचे देखें) और लागू होने पर टेक्स्ट विवरण होते हैं। यदि कम से कम एक रेडैक्शन विफल हो जाता है, तो आप [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) देखेंगे:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) पर क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

[RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) एनेमरेशन की सभी संभावित स्थितियाँ इस तालिका में सूचीबद्ध हैं:

| स्थिति | विवरण | संभावित कारण |
| --- | --- | --- |
| *Applied* | रेडैक्शन पूरी तरह और सफलतापूर्वक लागू किया गया | रेडैक्शन प्रक्रिया के भीतर सभी ऑपरेशन्स सफलतापूर्वक लागू किए गए |
| *PartiallyApplied* | रेडैक्शन केवल उसके मिलानों के एक हिस्से पर लागू किया गया | 1) प्रतिस्थापनों के लिए ट्रायल सीमाएँ पार हो गईं 2) कम से कम एक परिवर्तन उपयोगकर्ता द्वारा अस्वीकार किया गया |
| *Skipped* | रेडैक्शन को छोड़ दिया गया (लागू नहीं किया गया) | 1) रेडैक्शन के लिए ट्रायल सीमाएँ पार हो गईं 2) इस प्रकार के दस्तावेज़ पर रेडैक्शन लागू नहीं किया जा सकता 3) सभी प्रतिस्थापनों को उपयोगकर्ता द्वारा अस्वीकार किया गया और कोई परिवर्तन नहीं किया गया |
| *Failed* | रेडैक्शन अपवाद के साथ विफल हुआ | रेडैक्शन प्रक्रिया में एक अपवाद हुआ |

विस्तृत जानकारी के लिए आपको [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) में रेडैक्शन लॉग एंट्रीज़ को इटररेट करना होगा और *Applied* के अलावा किसी भी स्थिति वाले आइटम की [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) प्रॉपर्टी की जाँच करनी होगी:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # डिफ़ॉल्ट रूप से, रेडैक्टेड दस्तावेज़ PDF फ़ॉर्मेट में सहेजा जाता है
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # सभी विफल या छोड़े गए रेडैक्शन को डंप करें
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

आप एक ही कॉल में [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) मेथड को कॉल करके जितने भी रेडैक्शन की आवश्यकता हो, उतने लागू कर सकते हैं, क्योंकि इसका ओवरलोड रेडैक्शन और रेडैक्शन नीति की एक एरे स्वीकार करता है। इस स्थिति में, रेडैक्शन उसी क्रम में लागू होंगे जैसा कि एरे में दिखाया गया है। अपने कोड में रेडैक्शन सेट निर्दिष्ट करने के वैकल्पिक रूप में, आप रेडैक्शन नीति के साथ एक XML फ़ाइल बना सकते हैं, जैसा कि [यहाँ](). में वर्णित है।

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # लागू करने के लिए क्रम में रेडैक्शन की सूची प्रदान करें
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन की सूची लागू करें
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # डिफ़ॉल्ट रूप से, रेडैक्टेड दस्तावेज़ PDF फ़ॉर्मेट में सहेजा जाता है
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # सभी विफल या छोड़े गए रेडैक्शन को डंप करें
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) पर क्लिक करें।

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
