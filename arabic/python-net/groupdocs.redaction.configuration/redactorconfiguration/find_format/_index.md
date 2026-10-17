---
title: "طريقة find_format"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يبحث عن تكوينات الصيغ لامتداد ملف معين."
type: docs
url: /ar/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

يبحث عن تكوينات الصيغ لامتداد ملف معين.

```python
def find_format(self, file_extension):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| file_extension | `str` | امتداد الملف، الصيغة هي ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### مثال

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# احصل على نسخة التكوين المفردة
config = RedactorConfiguration.get_instance()

# استرجع إعدادات الصيغة لامتداد معين
settings = config.find_format(".txt")
if settings:
    # قم بتمديد قائمة الامتدادات المعالجة، على سبيل المثال، أضف .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### انظر أيضًا
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
