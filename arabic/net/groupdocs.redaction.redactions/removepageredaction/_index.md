---
title: RemovePageRedaction
second_title: GroupDocs.Redaction لمرجع .NET API
description: يمثل تنقيحًا يزيل صفحة شريحة  ورقة عمل  إلخ من المستند.
type: docs
weight: 610
url: /ar/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

يمثل تنقيحًا يزيل صفحة (شريحة ، ورقة عمل ، إلخ) من المستند.

```csharp
public class RemovePageRedaction : Redaction
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | تهيئة مثيل جديد لفئة RemovePageRedaction. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | الحصول على عدد الصفحات المراد إزالتها . |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | إرجاع سلسلة تصف التنقيح ومعلماته. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | يحصل على مؤشر موضع البداية (على أساس 0) . |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | الحصول على موضع مرجعي ، بداية المستند أو نهايته. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | يطبق التنقيح على مثيل تنسيق معين. |

### ملاحظات

**يتعلم أكثر**

* مزيد من التفاصيل حول تطبيق التنقيحات: [أساسيات التنقيح](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* مزيد من التفاصيل حول إزالة الصفحات: [إزالة تنقيح الصفحة](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### أمثلة

يوضح المثال التالي كيفية إزالة الصفحة الأخيرة من المستند.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### أنظر أيضا

* class [Redaction](../../groupdocs.redaction/redaction)
* مساحة الاسم [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* المجسم [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
