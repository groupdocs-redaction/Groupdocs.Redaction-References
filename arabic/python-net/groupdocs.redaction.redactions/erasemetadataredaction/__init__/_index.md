---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "ينشئ مثيلًا جديدًا من الفئة EraseMetadataRedaction، مما يمسح جميع البيانات الوصفية."
type: docs
url: /ar/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/
is_root: false
weight: 10
---


## __init__

ينشئ مثيلًا جديدًا من الفئة EraseMetadataRedaction، مما يمسح جميع البيانات الوصفية.

```python
def __init__(self):
    ...
```

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    redactor.save()
```

## __init__ {#filter}

يُنشئ مثيلاً جديدًا من EraseMetadataRedaction، يمسح البيانات الوصفية التي تطابق `MetadataFilters` المحددة.

```python
def __init__(self, filter):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| filter | `MetadataFilters` | تصفية للبيانات الوصفية المراد مسحها. |

### مثال

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # مسح جميع البيانات الوصفية
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # مسح حقل البيانات الوصفية للمؤلف فقط
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### انظر أيضًا
* class [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/)
