---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "निर्मित और कस्टम उपयोगकर्ता फ़ॉर्मेट सहित समर्थित फ़ॉर्मेट की सूची तक पहुँच प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.redaction.configuration/redactorconfiguration/
---
**Inheritance:**
java.lang.Object
```
public class RedactorConfiguration
```

निर्मित और कस्टम उपयोगकर्ता स्वरूपों सहित समर्थित स्वरूपों की सूची तक पहुँच प्रदान करता है।

*** ** * ** ***


**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](../https://docs.groupdocs.com/redaction/java/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](../https://docs.groupdocs.com/redaction/java/create-custom-format-handler/)

<br />

निम्नलिखित उदाहरण दिखाता है कि कैसे एक कस्टम उपयोगकर्ता फ़ॉर्मेट हैंडलर जोड़ा जाए।

````

  DocumentFormatConfiguration adobePhotoshopSettings = new DocumentFormatConfiguration();
 adobePhotoshopSettings.setExtensionFilter(".psd");
 adobePhotoshopSettings.setDocumentType(MyAdobePhotoshopFormatInstance.class);
 RedactorConfiguration configuration = RedactorConfiguration.getInstance();
 configuration.getAvailableFormats().add(adobePhotoshopSettings);
 
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
| [RedactorConfiguration()](#RedactorConfiguration--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getAvailableFormats()](#getAvailableFormats--) | Gets a list of recognized formats, see 
DocumentFormatConfiguration
.
 |
| [findFormat(String fileExtension)](#findFormat-java.lang.String-) | Finds format configurations for a given file extension.
 |
### RedactorConfiguration() {#RedactorConfiguration--}
```
public RedactorConfiguration()
```


### getAvailableFormats() {#getAvailableFormats--}
```
public final List<DocumentFormatConfiguration> getAvailableFormats()
```


Gets a list of recognized formats, see 
DocumentFormatConfiguration
.


**Returns:**
java.util.List<com.groupdocs.redaction.configuration.DocumentFormatConfiguration> - A list of recognized formats, see  DocumentFormatConfiguration .

### findFormat(String fileExtension) {#findFormat-java.lang.String-}
```
public final DocumentFormatConfiguration findFormat(String fileExtension)
```


Finds format configurations for a given file extension.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileExtension | java.lang.String | File extension, format is ".ext"
 |

**Returns:**
[DocumentFormatConfiguration](../../com.groupdocs.redaction.configuration/documentformatconfiguration) - If found, instance of  DocumentFormatConfiguration , null otherwise

