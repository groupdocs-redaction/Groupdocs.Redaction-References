---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل قائمة بأكثر أنواع البيانات الوصفية شيوعًا للمستند."
type: docs
weight: 19
url: /ar/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

يمثل قائمة بأكثر أنواع البيانات الوصفية شيوعًا للمستند.

## المُنشئات

| المُنشئ | الوصف |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [None](#None) | إعداد مرشح فارغ، لا يطابق أي عناصر بيانات وصفية. |
|
|  | [Author](#Author) | مؤلف المستند. |
|
|  | [Category](#Category) | فئة المستند. |
|
|  | [Comments](#Comments) | تعليق على المستند. |
|
|  | [Company](#Company) | شركة المؤلف. |
|
|  | [ContentStatus](#ContentStatus) | حالة المحتوى. |
|
|  | [CreatedTime](#CreatedTime) | وقت الإنشاء. |
|
|  | [HyperlinkBase](#HyperlinkBase) | قاعدة الرابط التشعبي. |
|
|  | [LastPrinted](#LastPrinted) | تاريخ ووقت الطباعة الأخيرة. |
|
|  | [LastSavedBy](#LastSavedBy) | آخر حفظ بواسطة المستخدم. |
|
|  | [LastSavedTime](#LastSavedTime) | تاريخ ووقت الحفظ الأخير. |
|
|  | [NameOfApplication](#NameOfApplication) | اسم التطبيق الذي تم إنشاء المستند فيه. |
|
|  | [Manager](#Manager) | اسم مدير المؤلف. |
|
|  | [RevisionNumber](#RevisionNumber) | رقم المراجعة. |
|
|  | [Subject](#Subject) | موضوع المستند. |
|
|  | [Template](#Template) | اسم قالب المستند. |
|
|  | [Title](#Title) | عنوان المستند. |
|
|  | [TotalEditingTime](#TotalEditingTime) | إجمالي وقت التحرير. |
|
|  | [Version](#Version) | إصدار المستند. |
|
|  | [Description](#Description) | وصف المستند. |
|
|  | [Keywords](#Keywords) | كلمات مفتاحية للمستند. |
|
|  | [ContentType](#ContentType) | نوع المحتوى. |
|
|  | [All](#All) | جميع أنواع عناصر البيانات الوصفية. |
|
## الطرق

| طريقة | الوصف |
| --- | --- |
|  | [getNames()](#getNames--) | يحصل على مجموعة تحتوي على جميع أنواع الفلاتر المعلنة. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | يحصل على قيمة MetadataFiler حسب اسمه. |
|
|  | [parse(String values)](#parse-java.lang.String-) | يقوم بتحليل سلسلة من القيم المفصولة بفواصل لـ MetadataFilers إلى عدد صحيح. |
|
|  | [toString(int value)](#toString-int-) | يحفظ عددًا صحيحًا كسلسلة من قيم MetadataFilers المفصولة بفواصل. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


إعداد مرشح فارغ، لا يطابق أي عناصر بيانات وصفية.


### Author {#Author}
```
public static final int Author
```


مؤلف المستند.


### Category {#Category}
```
public static final int Category
```


فئة المستند.


### Comments {#Comments}
```
public static final int Comments
```


تعليق على المستند.


### Company {#Company}
```
public static final int Company
```


شركة المؤلف.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


حالة المحتوى.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


وقت الإنشاء.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


قاعدة الرابط التشعبي.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


تاريخ ووقت الطباعة الأخيرة.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


آخر حفظ بواسطة المستخدم.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


تاريخ ووقت الحفظ الأخير.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


اسم التطبيق الذي تم إنشاء المستند فيه.


### Manager {#Manager}
```
public static final int Manager
```


اسم مدير المؤلف.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


رقم المراجعة.


### Subject {#Subject}
```
public static final int Subject
```


موضوع المستند.


### Template {#Template}
```
public static final int Template
```


اسم قالب المستند.


### Title {#Title}
```
public static final int Title
```


عنوان المستند.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


إجمالي وقت التحرير.


### Version {#Version}
```
public static final int Version
```


إصدار المستند.


### Description {#Description}
```
public static final int Description
```


وصف المستند.


### Keywords {#Keywords}
```
public static final int Keywords
```


كلمات مفتاحية للمستند.


### ContentType {#ContentType}
```
public static final int ContentType
```


نوع المحتوى.


### All {#All}
```
public static final int All
```


جميع أنواع عناصر البيانات الوصفية.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


يحصل على مجموعة تحتوي على جميع أنواع الفلاتر المعلنة.


**Returns:**
java.util.Set<java.lang.String> - مجموعة تحتوي على جميع أنواع الفلاتر المعلنة.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


يحصل على قيمة MetadataFiler حسب اسمه.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | valueName | java.lang.String | اسم MetadataFilter. |
|

**Returns:**
int - قيمة MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


يقوم بتحليل سلسلة من القيم المفصولة بفواصل لـ MetadataFilers إلى عدد صحيح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | values | java.lang.String | سلسلة من قيم MetadataFilers المفصولة بفواصل. |
|

**Returns:**
int - قيمة MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


يحفظ عددًا صحيحًا كسلسلة من قيم MetadataFilers المفصولة بفواصل.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | القيمة | int | قيمة MetadataFiler. |
|

**Returns:**
java.lang.String - سلسلة من قيم MetadataFiler المفصولة بفواصل.

