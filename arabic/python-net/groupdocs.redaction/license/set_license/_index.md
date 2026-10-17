---
title: "طريقة set_license"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "تطبيق ترخيص على العملية الحالية."
type: docs
url: /ar/python-net/groupdocs.redaction/license/set_license/
is_root: false
weight: 1010
---


## set_license {#license_source}

تطبيق ترخيص على العملية الحالية.

```python
def set_license(self, license_source):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| license_source |  | إما مسار سلسلة إلى ملف ``.lic`` أو كائن شبيه بالملف قابل للقراءة يُعيد بايتات الترخيص. يتم كتابة المدخلات الشبيهة بالملف إلى ملف مؤقت قبل تمريره إلى الجسر. |

| يُثير | الوصف |
| :- | :- |
| `TypeError` | إذا كان ``license_source`` ليس مسار سلسلة ولا كائن شبيه بالملف قابل للقراءة. |

### انظر أيضًا
* class [`License`](/redaction/python-net/groupdocs.redaction/license/)
