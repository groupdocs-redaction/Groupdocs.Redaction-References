---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "Redactor वर्ग की Apply विधि को पास किए गए रेडैक्शन की सूची के परिणामों का प्रतिनिधित्व करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Redactor वर्ग की Apply() विधि को पास किए गए रेडैक्शन की सूची के परिणामों का प्रतिनिधित्व करता है
Redactor
क्लास।

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | RedactorChangeLog क्लास का एक नया उदाहरण आरंभ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getStatus()](#getStatus--) | सभी लागू किए गए रेडैक्शन की अंतिम स्थिति प्राप्त करता है। |
|
|  | [getRedactionLog()](#getRedactionLog--) | सूची प्राप्त करता है |
RedactorLogEntry
इंस्टेंस।
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


RedactorChangeLog क्लास का एक नया उदाहरण आरंभ करता है।


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


सभी लागू किए गए रेडैक्शन की अंतिम स्थिति प्राप्त करता है।


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


सूची प्राप्त करता है
RedactorLogEntry
इंस्टेंस।


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - RedactorLogEntry इंस्टेंस की सूची।

