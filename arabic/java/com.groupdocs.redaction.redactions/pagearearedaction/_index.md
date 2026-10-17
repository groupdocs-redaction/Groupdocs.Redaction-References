---
title: "PageAreaRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل إخفاء نصي معقد يؤثر على صور النص والتعليقات التوضيحية في منطقة من الصفحة."
type: docs
weight: 23
url: /ar/java/com.groupdocs.redaction.redactions/pagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction), [com.groupdocs.redaction.redactions.RegexRedaction](../../com.groupdocs.redaction.redactions/regexredaction)
```
public class PageAreaRedaction extends RegexRedaction
```

يمثل إزالة نصية معقدة تؤثر على النصوص والصور والتعليقات التوضيحية في منطقة من الصفحة.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](../https://docs.groupdocs.com/redaction/java/use-page-area-redaction/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | ينشئ مثيلاً جديدًا لفئة PageAreaRedaction. |
|
|  | [PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)](#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | ينشئ مثيلاً جديدًا لفئة PageAreaRedaction. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getImageOptions()](#getImageOptions--) | يحصل على |
RegionReplacementOptions
خيارات مع معلمات اللون والمنطقة.
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | يطبق الحذف على نسخة تنسيق معينة. |
|
### PageAreaRedaction(Pattern regex, ReplacementOptions options) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options)
```


ينشئ مثيلاً جديدًا لفئة PageAreaRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | تعبير نمطي | java.util.regex.Pattern | تعبير نمطي للبحث والاستبدال |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|

### PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions) {#PageAreaRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public PageAreaRedaction(Pattern regex, ReplacementOptions options, RegionReplacementOptions imageOptions)
```


ينشئ مثيلاً جديدًا لفئة PageAreaRedaction.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | تعبير نمطي | java.util.regex.Pattern | تعبير نمطي للبحث والاستبدال |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | خيارات الاستبدال (نصية، لون) |
|
|  | imageOptions | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | خيارات الاستبدال (منطقة الصورة) |
|

### getImageOptions() {#getImageOptions--}
```
public final RegionReplacementOptions getImageOptions()
```


يحصل على
RegionReplacementOptions
خيارات مع معلمات اللون والمنطقة.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

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

