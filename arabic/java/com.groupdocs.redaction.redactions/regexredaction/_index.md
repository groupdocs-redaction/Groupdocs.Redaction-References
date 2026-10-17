---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل إزالة نصية تبحث وتستبدل النص في المستند عن طريق مطابقة التعبير النمطي المقدم."
type: docs
weight: 28
url: /ar/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

يمثل إزالة نصية تبحث وتستبدل النص في المستند عن طريق مطابقة التعبير النمطي المقدم.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | يُهيئ مثلاً جديداً من الفئة RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | يُهيئ مثلاً جديداً من الفئة RegexRedaction. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | يحصل على التعبير النمطي للمطابقة. |
|
|  | [getDescription()](#getDescription--) | يرجع سلسلة نصية تصف الحذف ومعامِلاته. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


يُهيئ مثلاً جديداً من الفئة RegexRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | نمط | java.lang.String | تعبير نمطي للبحث والاستبدال |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


يُهيئ مثلاً جديداً من الفئة RegexRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | تعبير نمطي | java.util.regex.Pattern | تعبير نمطي للبحث والاستبدال |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


يحصل على التعبير النمطي للمطابقة.


**Returns:**
java.util.regex.Pattern - التعبير النمطي للمطابقة.

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

