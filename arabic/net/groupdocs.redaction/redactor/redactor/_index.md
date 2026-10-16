---
title: "Redactor"
second_title: "GroupDocs.Redaction لـ .NET مرجع API"
description: "يُنشئ مثيلاً جديداً من الفئة Redactorgroupdocs.redaction/redactor باستخدام مسار الملف."
type: docs
weight: 10
url: /ar/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

يُنشئ مثيلاً جديداً من الفئة [`Redactor`](../../redactor) باستخدام مسار الملف.

```csharp
public Redactor(string filePath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف |

### أمثلة

المثال التالي يوضح كيفية فتح مستند للمعالجة.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // هنا يمكننا استخدام مثيل المستند لتنفيذ الإخفاءات
}
```

### انظر أيضًا

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

يُنشئ مثيلاً جديداً من الفئة [`Redactor`](../../redactor) باستخدام الدفق.

```csharp
public Redactor(Stream document)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مستند | Stream | دفق المصدر للمستند |

### أمثلة

المثال التالي يوضح كيفية فتح مستند من الدفق.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // هنا يمكننا استخدام مثيل المستند لتنفيذ الإخفاءات
    }
}
```

### انظر أيضًا

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

يُنشئ مثيلاً جديداً من الفئة [`Redactor`](../../redactor) لمستند محمي بكلمة مرور باستخدام مساره.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار إلى الملف. |
| loadOptions | LoadOptions | خيارات، بما في ذلك كلمة المرور. |

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

يُنشئ مثيلاً جديداً من الفئة [`Redactor`](../../redactor) لمستند محمي بكلمة مرور باستخدام مساره وإعداداته.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار إلى الملف. |
| loadOptions | LoadOptions | خيارات تعتمد على الملف، بما في ذلك كلمة المرور. |
| الإعدادات | RedactorSettings | الإعدادات الافتراضية لعملية التمويه. |

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

يُنشئ مثيلاً جديداً من الفئة [`Redactor`](../../redactor) لمستند محمي بكلمة مرور باستخدام الدفق.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مستند | Stream | دفق الإدخال المصدر. |
| loadOptions | LoadOptions | خيارات، بما في ذلك كلمة المرور. |

### أمثلة

يوضح المثال التالي كيفية فتح مستندات محمية بكلمة مرور باستخدام LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // هنا يمكننا استخدام مثيل المستند لتنفيذ الإخفاءات
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

يُنشئ مثيلاً جديدًا لفئة [`Redactor`](../../redactor) لمستند محمي بكلمة مرور باستخدام الدفق والإعدادات.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مستند | Stream | دفق الإدخال المصدر. |
| loadOptions | LoadOptions | خيارات، بما في ذلك كلمة المرور. |
| الإعدادات | RedactorSettings | الإعدادات الافتراضية لعملية التمويه. |

### أمثلة

يوضح المثال التالي كيفية فتح مستندات محمية بكلمة مرور باستخدام LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // هنا يمكننا استخدام مثيل المستند لتنفيذ الإخفاءات
}
```

### انظر أيضًا

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
