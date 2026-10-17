---
title: "EraseMetadataRedaction क्लास"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक मेटाडेटा रेडैक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ से सभी मेटाडेटा या विशिष्ट MetadataFilters से मेल खाने वाले मेटाडेटा को मिटा देता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

एक मेटाडेटा रेडैक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ से सभी मेटाडेटा या विशिष्ट MetadataFilters से मेल खाने वाले मेटाडेटा को मिटा देता है।

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

EraseMetadataRedaction प्रकार निम्नलिखित सदस्यों को उजागर करता है:

### निर्माता
| निर्माता | विवरण |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | EraseMetadataRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, सभी मेटाडेटा को मिटाते हुए। |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | EraseMetadataRedaction का एक नया उदाहरण प्रारंभ करता है, जो निर्दिष्ट `MetadataFilters` से मेल खाने वाले मेटाडेटा को मिटाता है। |

### विधियाँ
| विधि | विवरण |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | दिए गए फ़ॉर्मेट उदाहरण पर रेडैक्शन लागू करता है। (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### गुण
| गुण | विवरण |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | रेडैक्शन और उसके पैरामीटरों का विवरण। |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | सभी या विशिष्ट मेटाडेटा, जैसे Author या Company, चुनने के लिए उपयोग किया जाने वाला फ़िल्टर। (विरासत में मिला [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # सभी मेटाडेटा मिटाएँ
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # केवल author फ़ील्ड मिटाएँ
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
`EraseMetadataRedaction` का उपयोग करने वाले टास्क गाइड्स:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### संबंधित देखें
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
