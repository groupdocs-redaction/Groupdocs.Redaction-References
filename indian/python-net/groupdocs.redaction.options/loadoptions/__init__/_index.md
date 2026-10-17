---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "LoadOptions क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

LoadOptions क्लास का नया उदाहरण प्रारंभ करता है।

```python
def __init__(self):
    ...
```

## __init__ {#password}

निर्दिष्ट पासवर्ड के साथ LoadOptions का नया उदाहरण प्रारंभ करता है।

```python
def __init__(self, password):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| password | `str` | संरक्षित फ़ाइलों के लिए पासवर्ड। |

### उदाहरण

```python
    from groupdocs.redaction.options import LoadOptions

    # पासवर्ड‑सुरक्षित दस्तावेज़ लोड करें
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

निर्दिष्ट pre‑rasterization फ़्लैग के साथ नया LoadOptions उदाहरण प्रारंभ करता है।

```python
def __init__(self, pre_rasterize):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| pre_rasterize | `bool` | यदि True है, तो लोडिंग पर रास्टराइज़ेशन को बाध्य करें। |

## __init__ {#password-pre_rasterize}

निर्दिष्ट पासवर्ड के साथ नया LoadOptions उदाहरण प्रारंभ करता है।

यदि `pre_rasterize` True है, तो दस्तावेज़ लोड होने पर रास्टराइज़ेशन बाध्य किया जाता है।

```python
def __init__(self, password, pre_rasterize):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| password | `str` | संरक्षित फ़ाइलों के लिए पासवर्ड। |
| pre_rasterize | `bool` | यदि True है, तो लोडिंग पर रास्टराइज़ेशन को बाध्य करें। |

### उदाहरण

```python
from groupdocs.redaction.options import LoadOptions

# पासवर्ड‑सुरक्षित दस्तावेज़ लोड करें
load_opt = LoadOptions("mypassword")
```

### संबंधित देखें
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
