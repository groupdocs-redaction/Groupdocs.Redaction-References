---
title: "طريقة get_instance"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يعيد مثيلًا وحيدًا مع التكوين الافتراضي للصيغ المدمجة."
type: docs
url: /ar/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

يعيد مثيلًا وحيدًا مع التكوين الافتراضي للصيغ المدمجة.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### مثال

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# احصل على التكوين المفرد
config = RedactorConfiguration.get_instance()

# قم بتمديد الامتدادات المدعومة لتنسيقات النص العادي
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### انظر أيضًا
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
