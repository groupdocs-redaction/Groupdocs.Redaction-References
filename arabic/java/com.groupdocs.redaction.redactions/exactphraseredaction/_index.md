---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل تعديل نصي يستبدل العبارة الدقيقة في نص المستند دون حساسية لحالة الأحرف بشكل افتراضي."
type: docs
weight: 17
url: /ar/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

يمثل تشويهًا نصيًا يستبدل العبارة الدقيقة في نص المستند، غير حساس لحالة الأحرف بشكل افتراضي.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

المثال التالي يوضح تنفيذ بحث واستبدال العبارة مع حساسية حالة الأحرف.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// بشكل افتراضي، isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | ينشئ مثيلاً جديداً من الفئة ExactPhraseRedaction في وضع غير حساس لحالة الأحرف. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | ينشئ مثيلاً جديداً من الفئة ExactPhraseRedaction. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | يحصل على السلسلة للبحث والاستبدال. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | يحصل على قيمة تشير إلى ما إذا كان البحث حساسًا لحالة الأحرف أم لا. |
|
|  | [isRightToLeft()](#isRightToLeft--) | يحصل على قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | يضبط قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي. |
|
|  | [getDescription()](#getDescription--) | يرجع سلسلة نصية تصف الحذف ومعامِلاته. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


ينشئ مثيلاً جديداً من الفئة ExactPhraseRedaction في وضع غير حساس لحالة الأحرف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | السلسلة للبحث والاستبدال |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


ينشئ مثيلاً جديداً من الفئة ExactPhraseRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | السلسلة للبحث والاستبدال |
|
|  | isCaseSensitive | boolean | True إذا كان البحث حساسًا لحالة الأحرف مطلوب |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


يحصل على السلسلة للبحث والاستبدال.


**Returns:**
java.lang.String - السلسلة للبحث والاستبدال.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


يحصل على قيمة تشير إلى ما إذا كان البحث حساسًا لحالة الأحرف أم لا.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان البحث حساسًا لحالة الأحرف أم لا.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


يحصل على قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | boolean | قيمة تشير إلى ما إذا كان هذا النص من اليمين إلى اليسار أم لا، false بشكل افتراضي. |
|

### getDescription() {#getDescription--}
```
public String getDescription()
```


يرجع سلسلة نصية تصف الحذف ومعامِلاته.


**Returns:**
java.lang.String - نص يحتوي على اسم الحذف ومعامِلاته.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


يطبق الحذف على نسخة تنسيق معينة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | نسخة من مستند لتطبيق الحذف |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

