---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "MetadataSearchRedaction क्लास का एक नया उदाहरण आरंभ करता है, जो रेडैक्टेड आइटम्स से मेल खाने के लिए मान का उपयोग करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/metadatasearchredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#value_pattern-replacement}

MetadataSearchRedaction क्लास का एक नया उदाहरण आरंभ करता है, जो रेडैक्टेड आइटम्स से मेल खाने के लिए मान का उपयोग करता है।

```python
def __init__(self, value_pattern, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| value_pattern | `str` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति |
| replacement | `str` | पाठ्य प्रतिस्थापन |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    redactor.apply(MetadataSearchRedaction(".*@acme\\.com", "[EMAIL]"))
    redactor.save()
```

## __init__ {#value_pattern-replacement-key_pattern}

MetadataSearchRedaction का एक नया उदाहरण आरंभ करता है, जो आइटम नाम और मान का उपयोग करके रेडैक्टेड आइटम्स से मेल खाता है।

```python
def __init__(self, value_pattern, replacement, key_pattern):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| value_pattern | `str` | मेटाडाटा आइटम मान को खोजने और बदलने के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |
| key_pattern | `str` | मेटाडाटा आइटम नाम को खोजने और बदलने के लिए नियमित अभिव्यक्ति। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

with Redactor("document.docx") as redactor:
    # मेटाडाटा मानों में पाए गए किसी भी ईमेल पते को बदलें
    redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement}

MetadataSearchRedaction क्लास का एक नया उदाहरण आरंभ करता है, जो रेडैक्टेड आइटम्स से मेल खाने के लिए मान का उपयोग करता है।

```python
def __init__(self, value_regex, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | खोज और प्रतिस्थापन के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |

### उदाहरण

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import MetadataSearchRedaction

# मेटाडाटा में किसी भी ईमेल पते को रेडैक्ट करें
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

## __init__ {#value_regex-replacement-key_regex}

आइटम नाम और मान का उपयोग करके रेडैक्टेड आइटम्स से मेल खाने हेतु MetadataSearchRedaction का नया उदाहरण आरंभ करता है।

```python
def __init__(self, value_regex, replacement, key_regex):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| value_regex | `System.Text.RegularExpressions.Regex` | मेटाडाटा आइटम मान को खोजने और बदलने के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | पाठ्य प्रतिस्थापन। |
| key_regex | `System.Text.RegularExpressions.Regex` | मेटाडाटा आइटम नाम को खोजने और बदलने के लिए नियमित अभिव्यक्ति। |

### उदाहरण

```python
from groupdocs.redaction.redactions import MetadataSearchRedaction
from groupdocs.redaction import Redactor

# मेटाडाटा मानों में ईमेल पते को रेडैक्ट करें
redaction = MetadataSearchRedaction(r".*@acme\.com", "[EMAIL]")

with Redactor("document.docx") as redactor:
    redactor.apply(redaction)
    redactor.save()
```

### संबंधित देखें
* class [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/)
