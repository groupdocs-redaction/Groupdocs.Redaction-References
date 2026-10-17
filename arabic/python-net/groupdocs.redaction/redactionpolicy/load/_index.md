---
title: "طريقة load"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يقوم بتحميل RedactionPolicy من ملف XML."
type: docs
url: /ar/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

يقوم بتحميل RedactionPolicy من ملف XML.

```python
def load(cls, file_path):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_path | `str` | المسار إلى ملف XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### مثال

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

يقوم بتحميل مثيل RedactionPolicy من تدفق يحتوي على تكوين XML.

```python
def load(cls, input):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| input | `io.RawIOBase` | دفق يحتوي على تكوين XML. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### مثال

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# تحميل السياسة من ملف XML
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# تطبيق السياسة على مستند
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### انظر أيضًا
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
