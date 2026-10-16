---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक सैनिटाइज़ेशन नीति का प्रतिनिधित्व करता है जिसमें लागू करने के लिए विशिष्ट रिडैक्शन का एक सेट शामिल है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

सैनिटाइज़ेशन नीति का प्रतिनिधित्व करता है, जिसमें लागू करने के लिए विशिष्ट रिडैक्शन का सेट शामिल है।

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Redaction नीति का एक नया उदाहरण बनाता है। |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Redaction नीति का एक नया उदाहरण बनाता है जिसमें रिडैक्शन की एक विशिष्ट सूची होती है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | पूरी तरह कॉन्फ़िगर किए गए एक एरे प्राप्त करता है |
रिडैक्शन
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | एक उदाहरण लोड करता है |
RedactionPolicy
फ़ाइल पथ से।
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | एक उदाहरण लोड करता है |
RedactionPolicy
स्ट्रीम से।
|
|  | [save(String filePath)](#save-java.lang.String-) | रिडैक्शन नीति को फ़ाइल में सहेजता है। |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | रिडैक्शन नीति को स्ट्रीम में सहेजता है। |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Redaction नीति का एक नया उदाहरण बनाता है।


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Redaction नीति का एक नया उदाहरण बनाता है जिसमें रिडैक्शन की एक विशिष्ट सूची होती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | नीति के लिए रिडैक्शन का एक एरे |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


पूरी तरह कॉन्फ़िगर किए गए एक एरे प्राप्त करता है
रिडैक्शन
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - पूरी तरह कॉन्फ़िगर किए गए Redaction-व्युत्पन्न क्लासों का एक एरे।

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


एक उदाहरण लोड करता है
RedactionPolicy
फ़ाइल पथ से।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | XML फ़ाइल का पथ |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


एक उदाहरण लोड करता है
RedactionPolicy
स्ट्रीम से।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इनपुट | java.io.InputStream | XML कॉन्फ़िगरेशन वाली स्ट्रीम |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


रिडैक्शन नीति को फ़ाइल में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filePath | java.lang.String | फ़ाइल का पथ। |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


रिडैक्शन नीति को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | नीति को सहेजने के लिए लक्ष्य स्ट्रीम |
|

