---
title: "منشئ __init__"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "يُنشئ مثيلًا جديدًا من PreviewOptions."
type: docs
url: /ar/python-net/groupdocs.redaction.options/previewoptions/__init__/
is_root: false
weight: 10
---


## __init__ {#create_page_stream}

يُنشئ مثيلاً جديدًا من PreviewOptions. سيتم إغلاق تدفق الإخراج بعد الاستخدام.

```python
def __init__(self, create_page_stream):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | ينشئ تدفقًا لمعاينة صفحة محددة. |

## __init__ {#create_page_stream-release_page_stream}

يُنشئ مثيلاً جديدًا من PreviewOptions، مما يؤدي إلى إرجاع تدفق الإخراج إلى العميل للاستخدام لاحقًا.

```python
def __init__(self, create_page_stream, release_page_stream):
    ...
```

| معامل | النوع | الوصف |
| :- | :- | :- |
| create_page_stream | `CreatePageStream` | ينشئ تدفقًا لمعاينة صفحة محددة. |
| release_page_stream | `ReleasePageStream` | يُخطر بأن إنشاء معاينة الصفحة انتهى ويحصل على تدفق الإخراج. |

### انظر أيضًا
* class [`PreviewOptions`](/redaction/python-net/groupdocs.redaction.options/previewoptions/)
