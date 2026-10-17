---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل مرشح إخفاء يحدد منطقة داخل صفحة مستند لتطبيق الإخفاء."
type: docs
weight: 22
url: /ar/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

يمثل مرشح الإزالة، يحدد منطقة داخل صفحة من المستند لتطبيق الإزالة.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | ينشئ مثيلاً جديدًا لفئة PageAreaFilter لتطبيق الإخفاء على منطقة محددة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | يحصل على المستطيل (الموضع العلوي الأيسر وحجم المنطقة) في الصفحة. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | يتحقق مما إذا كانت منطقة هذا المرشح تتقاطع مع المستطيل المعطى. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


ينشئ مثيلاً جديدًا لفئة PageAreaFilter لتطبيق الإخفاء على منطقة محددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | topLeft | java.awt.Point | إحداثيات المنطقة العلوية اليسرى |
|
|  | size | java.awt.Dimension | حجم المنطقة واللون |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


يحصل على المستطيل (الموضع العلوي الأيسر وحجم المنطقة) في الصفحة.


**Returns:**
java.awt.Rectangle - المستطيل (الموضع العلوي الأيسر وحجم المنطقة) في الصفحة.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


يتحقق مما إذا كانت منطقة هذا المرشح تتقاطع مع المستطيل المعطى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | المستطيل للتحقق منه |
|

**Returns:**
boolean - true إذا كانت منطقة هذا المرشح تتقاطع

