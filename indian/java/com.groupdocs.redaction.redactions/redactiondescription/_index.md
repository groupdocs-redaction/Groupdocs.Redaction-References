---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "रिडैक्शन प्रक्रिया के दौरान किए गए एकल परिवर्तन कार्रवाई जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

रिडैक्शन प्रक्रिया के दौरान किए गए एकल परिवर्तन कार्रवाई जानकारी का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | RedactionDescription क्लास का नया इंस्टेंस बिना प्रतिस्थापन जानकारी के प्रारंभ करता है। |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | RedactionDescription क्लास का नया इंस्टेंस प्रतिस्थापन जानकारी के साथ प्रारंभ करता है। |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | RedactionDescription क्लास का नया इंस्टेंस इमेज एरिया प्रतिस्थापन जानकारी के साथ प्रारंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | दस्तावेज़ के डेटा प्रकार को प्राप्त करता है - टेक्स्ट, मेटाडेटा या एनोटेशन। |
|
|  | [getActionType()](#getActionType--) | रेडैक्शन ऑपरेशन प्राप्त करता है: प्रतिस्थापन, सफाई या हटाना। |
|
|  | [getOriginalText()](#getOriginalText--) | मिलते हुए पाठ को प्राप्त करता है, यदि कोई अभिव्यक्ति प्रदान की गई हो। |
|
|  | [getReplacement()](#getReplacement--) | प्रतिस्थापन जानकारी प्राप्त करता है, यह null हो सकता है। |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | छवि क्षेत्र रेडैक्शन के लिए प्रतिस्थापन जानकारी प्राप्त करता है, पाठ्य रेडैक्शन के लिए null लौटाता है। |
|
|  | [getDetails()](#getDetails--) | रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी प्राप्त करता है। |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी सेट करता है। |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


RedactionDescription क्लास का नया इंस्टेंस बिना प्रतिस्थापन जानकारी के प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redactionType | int | रेडैक्ट किए जा रहे डेटा का प्रकार |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | इन डेटा पर किए जाने वाले कार्य |
|
|  | originalText | java.lang.String | मिलता हुआ पाठ, टिप्पणी या एनोटेशन बॉडी |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


RedactionDescription क्लास का नया इंस्टेंस प्रतिस्थापन जानकारी के साथ प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redactionType | int | रेडैक्ट किए जा रहे डेटा का प्रकार |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | इन डेटा पर किए जाने वाले कार्य |
|
|  | originalText | java.lang.String | मिलता हुआ पाठ, टिप्पणी या एनोटेशन बॉडी |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | प्रतिस्थापन पाठ, मिलता हुआ पाठ और मूल स्ट्रिंग के भीतर उसकी स्थिति |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


RedactionDescription क्लास का नया इंस्टेंस इमेज एरिया प्रतिस्थापन जानकारी के साथ प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redactionType | int | रेडैक्ट किए जा रहे डेटा का प्रकार |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | इन डेटा पर किए जाने वाले कार्य |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | छवि क्षेत्र प्रतिस्थापन जानकारी |
|
|  | imageDetails | java.lang.String | छवि का पाठ्य विवरण, डिफ़ॉल्ट रूप से यह String.Empty है |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


दस्तावेज़ के डेटा प्रकार को प्राप्त करता है - टेक्स्ट, मेटाडेटा या एनोटेशन।


**Returns:**
int - दस्तावेज़ डेटा का प्रकार - पाठ, मेटाडेटा या एनोटेशन।

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


रेडैक्शन ऑपरेशन प्राप्त करता है: प्रतिस्थापन, सफाई या हटाना।


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


मिलते हुए पाठ को प्राप्त करता है, यदि कोई अभिव्यक्ति प्रदान की गई हो।


**Returns:**
java.lang.String - मिलता हुआ पाठ, यदि कोई अभिव्यक्ति प्रदान की गई हो।

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


प्रतिस्थापन जानकारी प्राप्त करता है, यह null हो सकता है।


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


छवि क्षेत्र रेडैक्शन के लिए प्रतिस्थापन जानकारी प्राप्त करता है, पाठ्य रेडैक्शन के लिए null लौटाता है।


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी प्राप्त करता है।


**Returns:**
java.lang.String - रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी।

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | रेडैक्ट किए जा रहे आइटम के लिए वैकल्पिक विवरण जानकारी। |
|

