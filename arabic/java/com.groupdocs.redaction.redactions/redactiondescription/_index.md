---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل معلومات إجراء تغيير واحد تم تنفيذها أثناء عملية الإزالة."
type: docs
weight: 25
url: /ar/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

يمثل معلومات إجراء تغيير واحد تم تنفيذها أثناء عملية الإزالة.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | ينشئ مثيلًا جديدًا من فئة RedactionDescription دون معلومات الاستبدال. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | ينشئ مثيلًا جديدًا من فئة RedactionDescription مع معلومات الاستبدال. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | ينشئ مثيلًا جديدًا من فئة RedactionDescription مع معلومات استبدال منطقة الصورة. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | يحصل على نوع بيانات المستند - النص أو البيانات الوصفية أو التعليقات التوضيحية. |
|
|  | [getActionType()](#getActionType--) | يحصل على عملية التمويه: الاستبدال أو التنظيف أو الحذف. |
|
|  | [getOriginalText()](#getOriginalText--) | يحصل على النص المطابق، إذا تم توفير أي تعبير. |
|
|  | [getReplacement()](#getReplacement--) | يحصل على معلومات الاستبدال، يمكن أن تكون فارغة. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | يحصل على معلومات الاستبدال لتمويهات منطقة الصورة، يرجع فارغًا لتمويهات النص. |
|
|  | [getDetails()](#getDetails--) | يحصل على معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | يضبط معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


ينشئ مثيلًا جديدًا من فئة RedactionDescription دون معلومات الاستبدال.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redactionType | int | نوع البيانات التي يتم تمويهها |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | الإجراء الذي سيُنفّذ على هذه البيانات |
|
|  | originalText | java.lang.String | النص المطابق، التعليق أو جسم الملاحظة |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


ينشئ مثيلًا جديدًا من فئة RedactionDescription مع معلومات الاستبدال.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redactionType | int | نوع البيانات التي يتم تمويهها |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | الإجراء الذي سيُنفّذ على هذه البيانات |
|
|  | originalText | java.lang.String | النص المطابق، التعليق أو جسم الملاحظة |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | نص الاستبدال، النص المطابق وموقعه داخل السلسلة الأصلية |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


ينشئ مثيلًا جديدًا من فئة RedactionDescription مع معلومات استبدال منطقة الصورة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | redactionType | int | نوع البيانات التي يتم تمويهها |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | الإجراء الذي سيُنفّذ على هذه البيانات |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | معلومات استبدال منطقة الصورة |
|
|  | imageDetails | java.lang.String | وصف نصي للصورة، بشكل افتراضي يكون String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


يحصل على نوع بيانات المستند - النص أو البيانات الوصفية أو التعليقات التوضيحية.


**Returns:**
int - نوع بيانات المستند - نص، بيانات وصفية أو ملاحظات.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


يحصل على عملية التمويه: الاستبدال أو التنظيف أو الحذف.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


يحصل على النص المطابق، إذا تم توفير أي تعبير.


**Returns:**
java.lang.String - النص المطابق، إذا تم توفير أي تعبير.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


يحصل على معلومات الاستبدال، يمكن أن تكون فارغة.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


يحصل على معلومات الاستبدال لتمويهات منطقة الصورة، يرجع فارغًا لتمويهات النص.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


يحصل على معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه.


**Returns:**
java.lang.String - معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


يضبط معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | معلومات تفاصيل اختيارية للعنصر الذي يتم تمويهه. |
|

