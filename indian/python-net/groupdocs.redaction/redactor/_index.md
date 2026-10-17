---
title: "रेडैक्टर क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक मुख्य क्लास को दर्शाता है जो दस्तावेज़ रेडैक्शन प्रक्रिया को नियंत्रित करती है, जिससे दस्तावेज़ खोलना, रेडैक्ट करना और सहेजना संभव होता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

एक मुख्य क्लास को दर्शाता है जो दस्तावेज़ रेडैक्शन प्रक्रिया को नियंत्रित करती है, जिससे दस्तावेज़ खोलना, रेडैक्ट करना और सहेजना संभव होता है।

और अधिक जानें
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

रेडैक्टर प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | फ़ाइल पथ का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | स्ट्रीम का उपयोग करके [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | पासवर्ड‑सुरक्षित दस्तावेज़ के लिए उसके पथ का उपयोग करके [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | पासवर्ड‑सुरक्षित दस्तावेज़ के लिए उसके पथ और सेटिंग्स का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | पासवर्ड‑सुरक्षित दस्तावेज़ के लिए स्ट्रीम का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड‑सुरक्षित दस्तावेज़ के लिए [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | दस्तावेज़ पर एक रेडैक्शन लागू करता है। |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | दस्तावेज़ पर रेडैक्शन का एक सेट लागू करता है। |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | दस्तावेज़ पर एक रेडैक्शन नीति लागू करता है। |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | संसाधनों को मुक्त करता है। |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | निर्दिष्ट छवि प्रारूप में विशिष्ट पृष्ठों की पूर्वावलोकन छवियों को उत्पन्न करता है। |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | दस्तावेज़ के बारे में सामान्य जानकारी प्राप्त करता है, जैसे आकार और पृष्ठ गिनती। |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | दस्तावेज़ को फ़ाइल में निम्नलिखित विकल्पों के साथ सहेजता है: AddSuffix = True, RasterizeToPDF = True। |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | दस्तावेज़ को फ़ाइल में सहेजता है। |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | कस्टम स्थान सहित दस्तावेज़ को स्ट्रीम में सहेजता है। |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# एक दस्तावेज़ खोलें और पहला पृष्ठ हटाएँ
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
`Redactor` का उपयोग करने वाले कार्य मार्गदर्शक:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### संबंधित देखें
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
