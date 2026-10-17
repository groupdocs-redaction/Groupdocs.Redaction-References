---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "एक regex पैटर्न और प्रतिस्थापन पाठ के साथ नया AnnotationRedaction प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/annotationredaction/__init__/
is_root: false
weight: 10
---


## __init__ {#pattern-replacement}

एक regex पैटर्न और प्रतिस्थापन पाठ के साथ नया AnnotationRedaction प्रारंभ करता है।

```python
def __init__(self, pattern, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| pattern | `str` | मैच करने के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | मैच किए गए टेक्स्ट के लिए पाठ प्रतिस्थापन। |

### उदाहरण

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# एनोटेशन टेक्स्ट में शब्द "approved" को रीडैक्ट करें
redaction = AnnotationRedaction(r"(?i)approved", "[REVIEW]")
```

## __init__ {#regex-replacement}

[`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) का नया उदाहरण प्रारंभ करता है।

```python
def __init__(self, regex, replacement):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | मैच करने के लिए नियमित अभिव्यक्ति। |
| replacement | `str` | मैच किए गए टेक्स्ट के लिए पाठ प्रतिस्थापन। |

### उदाहरण

```python
from groupdocs.redaction.redactions import AnnotationRedaction

# शब्द "approved" को (केस‑इंसेंसिटिव) रीडैक्ट करें और इसे "[REVIEW]" से बदलें।
redaction = AnnotationRedaction("(?i)approved", "[REVIEW]")
```

### संबंधित देखें
* class [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/)
