---
title: "MetadataSearchRedaction क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक मेटाडाटा रिडैक्शन को दर्शाता है जो नियमित अभिव्यक्तियों का उपयोग करके मेटाडाटा को खोजता और रिडैक्ट करता है, कुंजियों और/या मानों को मिलाते हुए।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/metadatasearchredaction/
is_root: false
weight: 140
---


## MetadataSearchRedaction class

एक मेटाडाटा रिडैक्शन को दर्शाता है जो नियमित अभिव्यक्तियों का उपयोग करके मेटाडाटा को खोजता और रिडैक्ट करता है, कुंजियों और/या मानों को मिलाते हुए।

- More details about applying redactions: <https://docs.groupdocs.com/redaction/net/redaction-basics/>
- More details about document metadata redactions: <https://docs.groupdocs.com/redaction/net/metadata-redactions/>

MetadataSearchRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement) | MetadataSearchRedaction क्लास का एक नया उदाहरण आरंभ करता है, जो रेडैक्टेड आइटम्स से मेल खाने के लिए मान का उपयोग करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_pattern-replacement-key_pattern) | MetadataSearchRedaction का एक नया उदाहरण आरंभ करता है, जो आइटम नाम और मान का उपयोग करके रेडैक्टेड आइटम्स से मेल खाता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement) | MetadataSearchRedaction क्लास का एक नया उदाहरण आरंभ करता है, जो रेडैक्टेड आइटम्स से मेल खाने के लिए मान का उपयोग करता है। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/#value_regex-replacement-key_regex) | आइटम नाम और मान का उपयोग करके रेडैक्टेड आइटम्स से मेल खाने हेतु MetadataSearchRedaction का नया उदाहरण आरंभ करता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/description/) | रेडैक्शन का विवरण, जिसमें उसका नाम और पैरामीटर शामिल हैं। |
| [key_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/key_expression/) | मेटाडाटा आइटम के नाम (की) से मेल खाने के लिए नियमित अभिव्यक्ति। |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/replacement/) | पाठ्य प्रतिस्थापन मान। |
| [value_expression](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/value_expression/) | मेटाडाटा आइटम के मान पाठ से मेल खाने के लिए नियमित अभिव्यक्ति। |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए उपयोग किया जाने वाला फ़िल्टर। (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # पैटर्न से मेल खाने वाले किसी भी मेटाडाटा मान को रेडैक्ट करें
    redaction = MetadataSearchRedaction("Company Ltd.", "--company--")
    redaction.filter = MetadataFilters.COMPANY
    redactor.apply(redaction)
    redactor.save()
```

### Guides
`MetadataSearchRedaction` का उपयोग करने वाले कार्य गाइड:

* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
