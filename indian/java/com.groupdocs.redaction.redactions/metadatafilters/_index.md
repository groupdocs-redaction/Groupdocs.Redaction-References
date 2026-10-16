---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "दस्तावेज़ मेटाडाटा के सबसे सामान्य प्रकारों की सूची को दर्शाता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

दस्तावेज़ मेटाडाटा के सबसे सामान्य प्रकारों की सूची को दर्शाता है।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
|  | [None](#None) | खाली फ़िल्टर सेटिंग, कोई भी मेटाडेटा आइटम नहीं मिलते। |
|
|  | [Author](#Author) | दस्तावेज़ के लेखक। |
|
|  | [Category](#Category) | दस्तावेज़ की श्रेणी। |
|
|  | [Comments](#Comments) | दस्तावेज़ के लिए टिप्पणी। |
|
|  | [Company](#Company) | लेखक की कंपनी। |
|
|  | [ContentStatus](#ContentStatus) | सामग्री की स्थिति। |
|
|  | [CreatedTime](#CreatedTime) | निर्माण समय। |
|
|  | [HyperlinkBase](#HyperlinkBase) | हाइपरलिंक आधार। |
|
|  | [LastPrinted](#LastPrinted) | अंतिम मुद्रित तिथि और समय। |
|
|  | [LastSavedBy](#LastSavedBy) | उपयोगकर्ता द्वारा अंतिम सहेजा गया। |
|
|  | [LastSavedTime](#LastSavedTime) | अंतिम सहेजी गई तिथि और समय। |
|
|  | [NameOfApplication](#NameOfApplication) | ऐप्लिकेशन का नाम जहाँ दस्तावेज़ बनाया गया था। |
|
|  | [Manager](#Manager) | लेखक के प्रबंधक का नाम। |
|
|  | [RevisionNumber](#RevisionNumber) | संशोधन संख्या। |
|
|  | [Subject](#Subject) | दस्तावेज़ का विषय। |
|
|  | [Template](#Template) | दस्तावेज़ टेम्पलेट का नाम। |
|
|  | [Title](#Title) | दस्तावेज़ शीर्षक। |
|
|  | [TotalEditingTime](#TotalEditingTime) | कुल संपादन समय। |
|
|  | [Version](#Version) | दस्तावेज़ का संस्करण। |
|
|  | [Description](#Description) | दस्तावेज़ का विवरण। |
|
|  | [Keywords](#Keywords) | दस्तावेज़ की कुंजीशब्द। |
|
|  | [ContentType](#ContentType) | सामग्री प्रकार। |
|
|  | [All](#All) | मेटाडेटा आइटम्स के सभी प्रकार। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getNames()](#getNames--) | सभी घोषित फ़िल्टर प्रकारों के सेट को प्राप्त करता है। |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | नाम द्वारा MetadataFiler का मान प्राप्त करता है। |
|
|  | [parse(String values)](#parse-java.lang.String-) | कॉमा-सेपरेटेड MetadataFilers मानों की स्ट्रिंग को int में पार्स करता है। |
|
|  | [toString(int value)](#toString-int-) | एक पूर्णांक को कॉमा-सेपरेटेड MetadataFilers मानों की स्ट्रिंग के रूप में सहेजता है। |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


खाली फ़िल्टर सेटिंग, कोई भी मेटाडेटा आइटम नहीं मिलते।


### Author {#Author}
```
public static final int Author
```


दस्तावेज़ के लेखक।


### Category {#Category}
```
public static final int Category
```


दस्तावेज़ की श्रेणी।


### Comments {#Comments}
```
public static final int Comments
```


दस्तावेज़ के लिए टिप्पणी।


### Company {#Company}
```
public static final int Company
```


लेखक की कंपनी।


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


सामग्री की स्थिति।


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


निर्माण समय।


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


हाइपरलिंक आधार।


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


अंतिम मुद्रित तिथि और समय।


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


उपयोगकर्ता द्वारा अंतिम सहेजा गया।


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


अंतिम सहेजी गई तिथि और समय।


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


ऐप्लिकेशन का नाम जहाँ दस्तावेज़ बनाया गया था।


### Manager {#Manager}
```
public static final int Manager
```


लेखक के प्रबंधक का नाम।


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


संशोधन संख्या।


### Subject {#Subject}
```
public static final int Subject
```


दस्तावेज़ का विषय।


### Template {#Template}
```
public static final int Template
```


दस्तावेज़ टेम्पलेट का नाम।


### Title {#Title}
```
public static final int Title
```


दस्तावेज़ शीर्षक।


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


कुल संपादन समय।


### Version {#Version}
```
public static final int Version
```


दस्तावेज़ का संस्करण।


### Description {#Description}
```
public static final int Description
```


दस्तावेज़ का विवरण।


### Keywords {#Keywords}
```
public static final int Keywords
```


दस्तावेज़ की कुंजीशब्द।


### ContentType {#ContentType}
```
public static final int ContentType
```


सामग्री प्रकार।


### All {#All}
```
public static final int All
```


मेटाडेटा आइटम्स के सभी प्रकार।


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


सभी घोषित फ़िल्टर प्रकारों के सेट को प्राप्त करता है।


**Returns:**
java.util.Set<java.lang.String> - सभी घोषित फ़िल्टर प्रकारों वाला एक सेट।

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


नाम द्वारा MetadataFiler का मान प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | valueName | java.lang.String | MetadataFilter का नाम। |
|

**Returns:**
int - MetadataFiler का मान।

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


कॉमा-सेपरेटेड MetadataFilers मानों की स्ट्रिंग को int में पार्स करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | values | java.lang.String | कॉमा-सेपरेटेड MetadataFilers मानों की एक स्ट्रिंग। |
|

**Returns:**
int - MetadataFilers का मान।

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


एक पूर्णांक को कॉमा-सेपरेटेड MetadataFilers मानों की स्ट्रिंग के रूप में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | MetadataFiler का मान। |
|

**Returns:**
java.lang.String - कॉमा-सेपरेटेड MetadataFiler मानों की एक स्ट्रिंग।

