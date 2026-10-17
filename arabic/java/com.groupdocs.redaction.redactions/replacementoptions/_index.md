---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل خيارات استبدال النص المطابق."
type: docs
weight: 31
url: /ar/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

يمثل خيارات استبدال النص المطابق.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | ينشئ مثيلًا جديدًا من فئة ReplacementOptions مع نص الاستبدال كخيار. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | ينشئ مثيلًا جديدًا من فئة ReplacementOptions مع مستطيل ملون كخيار. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getActionType()](#getActionType--) | يحصل على إجراء الاستبدال: رسم صندوق أو استبدال النص. |
|
|  | [getReplacement()](#getReplacement--) | يحصل على قيمة الاستبدال النصي. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | يضبط قيمة الاستبدال النصي. |
|
|  | [getBoxColor()](#getBoxColor--) | يحصل على اللون لـ |
ReplacementType.DrawBox
الخيار (يُهمل خلاف ذلك).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | يضبط اللون لـ |
ReplacementType.DrawBox
الخيار (يُهمل خلاف ذلك).
|
|  | [getFilters()](#getFilters--) | يحصل على مصفوفة من الفلاتر لتطبيقها مع هذا الحذف. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | يضبط مصفوفة من الفلاتر لتطبيقها مع هذا الحذف. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | يحصل على معالج حذف مخصص. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | يضبط معالج حذف مخصص. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


ينشئ مثيلًا جديدًا من فئة ReplacementOptions مع نص الاستبدال كخيار.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | استبدال | java.lang.String | استبدال نصي |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


ينشئ مثيلًا جديدًا من فئة ReplacementOptions مع مستطيل ملون كخيار.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | لون | java.awt.Color | لون المستطيل |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


يحصل على إجراء الاستبدال: رسم صندوق أو استبدال النص.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


يحصل على قيمة الاستبدال النصي.


**Returns:**
java.lang.String - قيمة الاستبدال النصي.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


يضبط قيمة الاستبدال النصي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.lang.String | قيمة الاستبدال النصي. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


يحصل على اللون لـ
ReplacementType.DrawBox
الخيار (يُهمل خلاف ذلك).


**Returns:**
java.awt.Color - اللون لخيار  ReplacementType.DrawBox  (يُهمل خلاف ذلك).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


يضبط اللون لـ
ReplacementType.DrawBox
الخيار (يُهمل خلاف ذلك).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | java.awt.Color | اللون لخيار  ReplacementType.DrawBox  (يُهمل خلاف ذلك). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


يحصل على مصفوفة من الفلاتر لتطبيقها مع هذا الحذف.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - مصفوفة من الفلاتر لتطبيقها مع هذا الحذف.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


يضبط مصفوفة من الفلاتر لتطبيقها مع هذا الحذف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | مصفوفة من الفلاتر لتطبيقها مع هذا الحذف. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


يحصل على معالج حذف مخصص. يدعم فقط ملفات PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


يضبط معالج حذف مخصص. يدعم فقط ملفات PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | مثال على [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
