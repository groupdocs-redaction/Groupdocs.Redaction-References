---
title: "टेक्स्ट रिडैक्शन"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख बताता है कि Python रिडैक्शन API आपको आपके दस्तावेज़ों से संवेदनशील या निजी डेटा को आसानी से रिडैक्ट करने की अनुमति कैसे देता है। आप विभिन्न फ़ॉर्मेट (जैसे PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX आदि) के दस्तावेज़ों के लिए सटीक वाक्यांश या रेगुलर एक्सप्रेशन का उपयोग करके टेक्स्ट रिडैक्शन लागू कर सकते हैं।"
type: docs
url: /hi/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction आपको आपके दस्तावेज़ों से संवेदनशील या निजी डेटा को आसानी से रिडैक्ट करने की सुविधा देता है। सबसे लोकप्रिय रिडैक्शन केस दस्तावेज़ से टेक्स्ट हटाना है।

GroupDocs.Redaction API के साथ आप विभिन्न फ़ॉर्मेट (जैसे PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX आदि) के दस्तावेज़ों के लिए सटीक वाक्यांश या [रेगुलर एक्सप्रेशन](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) का उपयोग करके टेक्स्ट रिडैक्शन लागू कर सकते हैं। पूर्ण सूची के लिए [supported document formats]() लेख देखें।

## Use exact phrase redaction

नीचे के उदाहरण में, हम टेक्स्ट रिडैक्शन लागू करते हैं, व्यक्तिगत सटीक वाक्यांश "John Doe" को "\\[personal\\]" (या किसी भी अपवाद कोड) से बदलते हैं:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

डिफ़ॉल्ट रूप से, सटीक वाक्यांश की खोज केस-सेंसिटिव नहीं होती। केस-सेंसिटिव रेडैक्शन के लिए, एक कंस्ट्रक्टर पैरामीटर और संबंधित सार्वजनिक प्रॉपर्टी मौजूद है:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # केस-सेंसिटिव मिलान सक्षम करें
    case_sensitive = True

    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

यदि आपको रेडैक्टेड टेक्स्ट के ऊपर एक रंगीन बॉक्स चाहिए, तो आप रिप्लेसमेंट स्ट्रिंग के बजाय रंग का उपयोग कर सकते हैं। रेडैक्शन मिलते हुए टेक्स्ट को मिटा देगा और रेडैक्टेड टेक्स्ट की जगह निर्दिष्ट रंग का आयताकार बॉक्स रखेगा:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) क्लिक करें।

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

आपको दाएँ‑से‑बाएँ लिखे दस्तावेज़, जैसे अरबी या हिब्रू, पर रेडैक्शन लागू करने की आवश्यकता हो सकती है। निम्नलिखित उदाहरण दिखाता है कि Arabic PDF दस्तावेज़ पर ExactPhraseRedaction कैसे लागू करें:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # अरबी वाक्यांश के साथ रेडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./arabic.pdf") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(ex_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` इस उदाहरण में उपयोग की गई सैंपल फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) क्लिक करें।

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

पर्दे के पीछे, \"सटीक वाक्यांश\" रेडैक्शन रेगुलर एक्सप्रेशन के माध्यम से काम करता है, जो रेडैक्शन का मूल तरीका है। नीचे दिए गए उदाहरण में, हम \"2 अंक, स्पेस या कुछ नहीं, 2 अंक, फिर स्पेस और 6 अंक\" से मेल खाने वाले किसी भी टेक्स्ट को नीले रंग के बॉक्स के साथ रेडैक्ट करते हैं:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # रिडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(reg_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

यदि आपको पूरे पैराग्राफ को रेडैक्ट करना है, तो आपको RegexRedaction का उपयोग भी करना पड़ सकता है। निम्नलिखित उदाहरण दिखाता है कि PDF दस्तावेज़ में पूरे पैराग्राफ को कैसे रेडैक्ट करें:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # रेडैक्शन बॉक्स का रंग निर्धारित करें
    color = Color.from_argb(255, 220, 20, 60)

    # पूरे पैराग्राफ से मेल खाने वाले रेडैक्शन विकल्प निर्दिष्ट करें
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.pdf") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(reg_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` इस उदाहरण में उपयोग की गई सैंपल फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) क्लिक करें।

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
