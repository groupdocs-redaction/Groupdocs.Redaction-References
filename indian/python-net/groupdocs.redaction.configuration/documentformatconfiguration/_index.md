---
title: "DocumentFormatConfiguration क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "DocumentFormatInstance-व्युत्पन्न क्लास के लिए एक टाइप रेफ़रेंस और तेज़ फ़ॉर्मेट पहचान के लिए समर्थित फ़ाइल एक्सटेंशन की सूची का प्रतिनिधित्व करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

एक प्रकार संदर्भ को दर्शाता है जो [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-व्युत्पन्न क्लास और तेज़ फ़ॉर्मेट पहचान के लिए समर्थित फ़ाइल एक्सटेंशन की सूची के लिए है।

और अधिक जानें

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatConfiguration प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | DocumentFormatConfiguration का एक नया इंस्टेंस प्रारंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | जाँचता है कि दिया गया फ़ाइल एक्सटेंशन DocumentType के रूप में संभाला जा सकता है। |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### गुण
| गुण | विवरण |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | एक क्लास का प्रकार जो [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) से विरासत में लेती है। |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | फ़ाइल एक्सटेंशन की कॉमा‑सेपरेटेड सूची (उदाहरण के लिए ".pdf"), केस‑इंसेंसिटिव। |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) प्रारंभिककरण के लिए आवश्यक डेटा। |

### उदाहरण

```python
from groupdocs.redaction import DocumentFormatConfiguration

# एक कस्टम फ़ॉर्मेट कॉन्फ़िगरेशन बनाएं
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### संबंधित देखें
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
