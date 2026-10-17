---
title: "load मेथड"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "XML फ़ाइल से एक RedactionPolicy लोड करता है।"
type: docs
url: /hi/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

XML फ़ाइल से एक RedactionPolicy लोड करता है।

```python
def load(cls, file_path):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| file_path | `str` | XML फ़ाइल का पथ। |

**Returns:** RedactionPolicy: The loaded redaction policy.

### उदाहरण

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

XML कॉन्फ़िगरेशन वाली स्ट्रीम से एक RedactionPolicy इंस्टेंस लोड करता है।

```python
def load(cls, input):
    ...
```

| पैरामीटर | प्रकार | विवरण |
| :- | :- | :- |
| input | `io.RawIOBase` | XML कॉन्फ़िगरेशन युक्त स्ट्रीम। |

**Returns:** RedactionPolicy: The loaded redaction policy.

### उदाहरण

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# XML फ़ाइल से नीति लोड करें
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# नीति को दस्तावेज़ पर लागू करें
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### संबंधित देखें
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
