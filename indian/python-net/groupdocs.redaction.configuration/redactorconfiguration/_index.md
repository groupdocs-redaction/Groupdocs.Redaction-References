---
title: "RedactorConfiguration क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "समर्थित फ़ॉर्मेट्स, बिल्ट‑इन और कस्टम उपयोगकर्ता फ़ॉर्मेट्स की सूची तक पहुँच प्रदान करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

समर्थित फ़ॉर्मेट्स, बिल्ट‑इन और कस्टम उपयोगकर्ता फ़ॉर्मेट्स की सूची तक पहुँच प्रदान करता है।

और अधिक जानें:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

RedactorConfiguration प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | दिए गए फ़ाइल एक्सटेंशन के लिए फ़ॉर्मेट कॉन्फ़िगरेशन खोजता है। |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | बिल्ट‑इन फ़ॉर्मेट्स की डिफ़ॉल्ट कॉन्फ़िगरेशन के साथ एक सिंगलटन इंस्टेंस लौटाता है। |

### गुण
| गुण | विवरण |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | पहचाने गए फ़ॉर्मेट्स की सूची, देखें [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### उदाहरण

```python
# एक कस्टम यूज़र फ़ॉर्मेट हैंडलर जोड़ें
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# एक बिल्ट‑इन या कस्टम यूज़र फ़ॉर्मेट हैंडलर प्राप्त करें
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### संबंधित देखें
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
