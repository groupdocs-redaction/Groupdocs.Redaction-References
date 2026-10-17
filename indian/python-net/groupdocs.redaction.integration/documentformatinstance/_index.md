---
title: "DocumentFormatInstance क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "किसी दस्तावेज़ के एक विशिष्ट फ़ॉर्मेट को दर्शाता है और कस्टम दस्तावेज़ प्रकार जोड़ने के लिए लागू किया जा सकता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

किसी दस्तावेज़ के एक विशिष्ट फ़ॉर्मेट को दर्शाता है और कस्टम दस्तावेज़ प्रकार जोड़ने के लिए लागू किया जा सकता है।

और अधिक जानें

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatInstance प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | दस्तावेज़ फ़ॉर्मेट हैंडलर उदाहरण को प्रारंभ करता है। |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) कार्यान्वयन की जाँच करता है और यदि निर्दिष्ट हो तो उसे बुलाता है। |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | स्ट्रीम से दस्तावेज़ लोड करता है। |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | जाँचता है कि दिया गया स्ट्रीम इस फ़ॉर्मेट उदाहरण द्वारा समर्थित दस्तावेज़ रखता है या नहीं। |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | दस्तावेज़ को स्ट्रीम में सहेजता है। |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | पासवर्ड-संरक्षित दस्तावेज़ों के लिए पासवर्ड। |

### उदाहरण

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # फ़ाइल सामग्री लोड करें
        pass

    def save(self, output: io.RawIOBase) -> None:
        # फ़ाइल में परिवर्तन सहेजें
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### संबंधित देखें
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
