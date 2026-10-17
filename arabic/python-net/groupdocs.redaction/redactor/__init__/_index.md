---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلًا جديدًا من Redactor باستخدام مسار ملف."
type: docs
url: /ar/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

ينشئ مثيلًا جديدًا من Redactor باستخدام مسار ملف.

```python
def __init__(self, file_path):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_path | `str` | المسار إلى الملف. |

### مثال

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # نفّذ عمليات الحذف هنا
    pass
```

## __init__ {#document}

ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) باستخدام تدفق.

```python
def __init__(self, document):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| document | `io.RawIOBase` | تدفق المصدر للمستند. |

### مثال

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # افتح الوثيقة كتيار ثنائي
    with open("./sample.pdf", "rb") as stream:
        # حمّل الوثيقة من التيار
        with Redactor(stream) as redactor:
            # نفّذ عمليات الحذف هنا
            pass
```

## __init__ {#file_path-load_options}

ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) لمستند محمي بكلمة مرور باستخدام مساره.

```python
def __init__(self, file_path, load_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_path | `str` | المسار إلى الملف. |
| load_options | `LoadOptions` | الخيارات، بما في ذلك كلمة المرور. |

### مثال

```python
from groupdocs.redaction import Redactor

# حمّل مستندًا محميًا بكلمة مرور من مسار ملف
with Redactor("protected.docx") as redactor:
    # نفّذ عمليات الحذف هنا
    pass
```

## __init__ {#file_path-load_options-settings}

ينشئ مثيلًا جديدًا من Redactor لمستند محمي بكلمة مرور باستخدام مساره والإعدادات.

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_path | `str` | المسار إلى الملف. |
| load_options | `LoadOptions` | خيارات تعتمد على الملف، بما في ذلك كلمة المرور. |
| settings | `RedactorSettings` | الإعدادات الافتراضية لعملية الحذف. |

### مثال

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

ينشئ مثيلًا جديدًا من Redactor لمستند محمي بكلمة مرور باستخدام تدفق.

```python
def __init__(self, document, load_options):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| document | `io.RawIOBase` | تدفق الإدخال المصدر. |
| load_options | `LoadOptions` | الخيارات، بما في ذلك كلمة المرور. |

### مثال

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # افتح ملف PDF المحمي كتيار ثنائي
    with open(r"C:\sample.pdf", "rb") as stream:
        # قدّم كلمة المرور عبر LoadOptions
        load_options = LoadOptions("mypassword")
        # ابدأ Redactor باستخدام التيار وخيارات التحميل
        with Redactor(stream, load_options) as redactor:
            # نفّذ عمليات الحذف هنا
            pass
```

## __init__ {#document-load_options-settings}

ينشئ مثيلًا جديدًا من [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) لمستند محمي بكلمة مرور باستخدام تدفق وإعدادات.

```python
def __init__(self, document, load_options, settings):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| document | `io.RawIOBase` | تدفق الإدخال المصدر. |
| load_options | `LoadOptions` | الخيارات، بما في ذلك كلمة المرور. |
| settings | `RedactorSettings` | الإعدادات الافتراضية لعملية الحجب. |

### انظر أيضًا
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
