---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُهيئ مثلاً جديداً من فئة LoadOptions."
type: docs
url: /ar/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

يُهيئ مثلاً جديداً من فئة LoadOptions.

```python
def __init__(self):
    ...
```

## __init__ {#password}

يُهيئ مثلاً جديداً من LoadOptions باستخدام كلمة المرور المحددة.

```python
def __init__(self, password):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| password | `str` | كلمة مرور للملفات المحمية. |

### مثال

```python
    from groupdocs.redaction.options import LoadOptions

    # تحميل مستند محمي بكلمة مرور
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

يُهيئ مثلاً جديداً من LoadOptions مع العلامة المحددة للتمهيد المسبق للتصوير النقطي.

```python
def __init__(self, pre_rasterize):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| pre_rasterize | `bool` | إذا كان True، فرض التحويل إلى نقطية عند التحميل. |

## __init__ {#password-pre_rasterize}

يُهيئ مثلاً جديداً من LoadOptions مع كلمة المرور المحددة.

إذا كان `pre_rasterize` True، يتم فرض التحويل إلى نقطية عندما يتم تحميل المستند.

```python
def __init__(self, password, pre_rasterize):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| password | `str` | كلمة مرور للملفات المحمية. |
| pre_rasterize | `bool` | إذا كان True، فرض التحويل إلى نقطية عند التحميل. |

### مثال

```python
from groupdocs.redaction.options import LoadOptions

# تحميل مستند محمي بكلمة مرور
load_opt = LoadOptions("mypassword")
```

### انظر أيضًا
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
