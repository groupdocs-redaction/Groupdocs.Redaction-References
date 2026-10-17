---
title: "__init__ कन्स्ट्रक्टर"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "फ़ाइल पथ का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

फ़ाइल पथ का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, file_path):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_path | `str` | फ़ाइल का पाथ। |

### उदाहरण

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # यहाँ रेडैक्शन ऑपरेशन्स करें
    pass
```

## __init__ {#document}

स्ट्रीम का उपयोग करके [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, document):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| document | `io.RawIOBase` | दस्तावेज़ का सोर्स स्ट्रीम। |

### उदाहरण

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # दस्तावेज़ को बाइनरी स्ट्रीम के रूप में खोलें
    with open("./sample.pdf", "rb") as stream:
        # स्ट्रीम से दस्तावेज़ लोड करें
        with Redactor(stream) as redactor:
            # यहाँ रेडैक्शन करें
            pass
```

## __init__ {#file_path-load_options}

पासवर्ड‑सुरक्षित दस्तावेज़ के लिए उसके पथ का उपयोग करके [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, file_path, load_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_path | `str` | फ़ाइल का पाथ। |
| load_options | `LoadOptions` | ऑप्शन, जिसमें पासवर्ड शामिल है। |

### उदाहरण

```python
from groupdocs.redaction import Redactor

# फ़ाइल पाथ से पासवर्ड‑सुरक्षित दस्तावेज़ लोड करें
with Redactor("protected.docx") as redactor:
    # यहाँ रेडैक्शन ऑपरेशन्स करें
    pass
```

## __init__ {#file_path-load_options-settings}

पासवर्ड‑सुरक्षित दस्तावेज़ के लिए उसके पथ और सेटिंग्स का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_path | `str` | फ़ाइल का पथ। |
| load_options | `LoadOptions` | फ़ाइल‑निर्भर ऑप्शन, जिसमें पासवर्ड शामिल है। |
| settings | `RedactorSettings` | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### उदाहरण

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

पासवर्ड‑सुरक्षित दस्तावेज़ के लिए स्ट्रीम का उपयोग करके एक नया रेडैक्टर इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, document, load_options):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| document | `io.RawIOBase` | सोर्स इनपुट स्ट्रीम। |
| load_options | `LoadOptions` | ऑप्शन, जिसमें पासवर्ड शामिल है। |

### उदाहरण

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # प्रोटेक्टेड PDF को बाइनरी स्ट्रीम के रूप में खोलें
    with open(r"C:\sample.pdf", "rb") as stream:
        # LoadOptions के माध्यम से पासवर्ड प्रदान करें
        load_options = LoadOptions("mypassword")
        # स्ट्रीम और लोड ऑप्शन के साथ Redactor को इनिशियलाइज़ करें
        with Redactor(stream, load_options) as redactor:
            # यहाँ रेडैक्शन ऑपरेशन्स करें
            pass
```

## __init__ {#document-load_options-settings}

स्ट्रीम और सेटिंग्स का उपयोग करके पासवर्ड‑सुरक्षित दस्तावेज़ के लिए [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) का एक नया इंस्टेंस प्रारंभ करता है।

```python
def __init__(self, document, load_options, settings):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| document | `io.RawIOBase` | सोर्स इनपुट स्ट्रीम। |
| load_options | `LoadOptions` | ऑप्शन, जिसमें पासवर्ड शामिल है। |
| settings | `RedactorSettings` | रेडैक्शन प्रक्रिया के लिए डिफ़ॉल्ट सेटिंग्स। |

### संबंधित देखें
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
