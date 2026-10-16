---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "يمثل تشويهًا للبيانات الوصفية يمحو جميع البيانات الوصفية أو البيانات الوصفية التي تطابق MetadataFilters المحددة من المستند."
type: docs
weight: 16
url: /ar/java/com.groupdocs.redaction.redactions/erasemetadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.MetadataRedaction](../../com.groupdocs.redaction.redactions/metadataredaction)
```
public class EraseMetadataRedaction extends MetadataRedaction
```

يمثل تشويهًا للبيانات الوصفية يمحو جميع البيانات الوصفية أو البيانات الوصفية التي تطابق MetadataFilters المحددة من المستند.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />

المثال التالي يوضح كيفية مسح (تعيين قيم فارغة) جميع البيانات الوصفية أو بعضها.

````

  try (Redactor redactor = new Redactor("C:\\sample.docx"))
 {
    // Erase Author, Manager and Company
    redactor.apply(new EraseMetadataRedaction(MetadataFilters.Author | MetadataFilters.Manager | MetadataFilters.Company));
    // Erase all metadata
    redactor.apply(new EraseMetadataRedaction(MetadataFilters.All));
    redactor.save();
 }
 
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
| [EraseMetadataRedaction()](#EraseMetadataRedaction--) | Initializes a new instance of EraseMetadataRedaction class, erasing all metadata.
 |
| [EraseMetadataRedaction(int filter)](#EraseMetadataRedaction-int-) | Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of 
MetadataFilters
.
 |
## Methods

| Method | Description |
| --- | --- |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters.
 |
### EraseMetadataRedaction() {#EraseMetadataRedaction--}
```
public EraseMetadataRedaction()
```


Initializes a new instance of EraseMetadataRedaction class, erasing all metadata.


### EraseMetadataRedaction(int filter) {#EraseMetadataRedaction-int-}
```
public EraseMetadataRedaction(int filter)
```


Initializes a new instance of EraseMetadataRedaction class, erasing metadata, matching specific combination of 
MetadataFilters
.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | int | Filter for metadata to erase
 |

### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.


**Returns:**
java.lang.String - Text, containing redaction name and parameters.

