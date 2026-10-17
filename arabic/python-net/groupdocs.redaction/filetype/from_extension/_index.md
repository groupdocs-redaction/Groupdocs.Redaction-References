---
title: "طريقة from_extension"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يربط امتداد الملف بنوع الملف."
type: docs
url: /ar/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

يربط امتداد الملف بنوع الملف.

```python
def from_extension(cls, extension):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| extension | `str` | امتداد الملف (بما في ذلك النقطة "."). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| يُثير | الوصف |
| :- | :- |
| `ValueError` | عند أن `extension` يساوي null أو سلسلة فارغة. |

### انظر أيضًا
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
