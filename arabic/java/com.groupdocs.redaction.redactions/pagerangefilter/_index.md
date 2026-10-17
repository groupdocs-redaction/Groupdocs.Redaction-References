---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل مرشح الإزالة الذي يحدد نطاق الصفحات داخل مستند لتطبيق الإزالة."
type: docs
weight: 24
url: /ar/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

يمثل مرشح الإزالة، يحدد نطاق الصفحات داخل المستند لتطبيق الإزالة.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | يُهيئ مثيلًا جديدًا من الفئة RemovePageRedaction. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | يحصل على موضع الإشارة المرجعية، بداية أو نهاية المستند. |
|
|  | [getIndex()](#getIndex--) | يحصل على فهرس موضع البداية (بدءًا من 0). |
|
|  | [getCount()](#getCount--) | يحصل على عدد الصفحات التي سيتم إزالتها. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | يتحقق مما إذا كان نطاق الصفحات لهذا المرشح يحتوي على الصفحة المحددة. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


يُهيئ مثيلًا جديدًا من الفئة RemovePageRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | موضع الإشارة المرجعية، بداية أو نهاية المستند |
|
|  | فهرس | int | فهرس موضع البداية (بدءًا من 0) |
|
|  | العدد | int | عدد الصفحات التي سيتم إزالتها |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


يحصل على موضع الإشارة المرجعية، بداية أو نهاية المستند.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


يحصل على فهرس موضع البداية (بدءًا من 0).


**Returns:**
int - فهرس موضع البداية (مبني على الصفر).

### getCount() {#getCount--}
```
public final int getCount()
```


يحصل على عدد الصفحات التي سيتم إزالتها.


**Returns:**
int - عدد الصفحات التي سيتم إزالتها.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


يتحقق مما إذا كان نطاق الصفحات لهذا المرشح يحتوي على الصفحة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pageIndex | int | فهرس الصفحة (مبني على الصفر) |
|
|  | pageCount | int | إجمالي عدد الصفحات |
|

**Returns:**
boolean - true إذا كان نطاق الفلتر يحتوي على صفحة

