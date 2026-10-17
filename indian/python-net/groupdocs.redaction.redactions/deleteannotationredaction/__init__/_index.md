---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जिसमें सभी एनोटेशन को हटाने की सेटिंग्स (सब कुछ मिलान) होती हैं।"
type: docs
url: /hi/python-net/groupdocs.redaction.redactions/deleteannotationredaction/__init__/
is_root: false
weight: 10
---


## __init__

DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जिसमें सभी एनोटेशन को हटाने की सेटिंग्स (सब कुछ मिलान) होती हैं।

```python
def __init__(self):
    ...
```

### उदाहरण

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# सभी एनोटेशन हटाएँ
del_red = DeleteAnnotationRedaction()
```

## __init__ {#pattern}

DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जो दिए गए अभिव्यक्ति से मेल खाने वाले एनोटेशन को हटाता है।

```python
def __init__(self, pattern):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| pattern | `str` | नियमित अभिव्यक्ति. |

### उदाहरण

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# ऐसे एनोटेशन हटाएँ जिनमें शब्द "internal" (बिना केस के) शामिल हो।
del_red = DeleteAnnotationRedaction(r"(?i)internal")
```

## __init__ {#regex}

DeleteAnnotationRedaction वर्ग का एक नया उदाहरण आरंभ करता है, जो दिए गए अभिव्यक्ति से मेल खाने वाले एनोटेशन को हटाता है।

```python
def __init__(self, regex):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| regex | `System.Text.RegularExpressions.Regex` | नियमित अभिव्यक्ति. |

### उदाहरण

```python
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

# उन एनोटेशन को हटाएँ जिनकी सामग्री रेगेक्स से मेल खाती है (case‑insensitive)
del_red = DeleteAnnotationRedaction("(?i)internal")
```

### संबंधित देखें
* class [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/)
