---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "EraseMetadataRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, सभी मेटाडेटा को मिटाते हुए।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

EraseMetadataRedaction क्लास का नया इंस्टेंस इनिशियलाइज़ करता है, सभी मेटाडेटा को मिटाते हुए।

```python
def __init__(self):
    ...
```

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

EraseMetadataRedaction का एक नया उदाहरण प्रारंभ करता है, जो निर्दिष्ट `MetadataFilters` से मेल खाने वाले मेटाडेटा को मिटाता है।

```python
def __init__(self, filter):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| filter | `MetadataFilters` | मेटाडेटा को मिटाने के लिए फ़िल्टर। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # सभी मेटाडेटा मिटाएँ
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # केवल लेखक मेटाडेटा फ़ील्ड को मिटाएँ
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### संबंधित देखें
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
