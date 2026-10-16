---
title: "RedactorConfiguration"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "내장 및 사용자 정의 형식의 지원 목록에 대한 접근을 제공합니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.redaction.configuration/redactorconfiguration/
---
**Inheritance:**
java.lang.Object
```
public class RedactorConfiguration
```

내장 및 사용자 정의 형식을 포함한 지원 형식 목록에 대한 접근을 제공합니다.

*** ** * ** ***


**Learn more**

* More details about **GroupDocs.Redaction** configuration: [Extend supported extensions list](../https://docs.groupdocs.com/redaction/java/extend-supported-extensions-list/)
* More details about implementing custom formats: [Create custom format handler](../https://docs.groupdocs.com/redaction/java/create-custom-format-handler/)

<br />

다음 예제는 사용자 정의 형식 핸들러를 추가하는 방법을 보여줍니다.

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

