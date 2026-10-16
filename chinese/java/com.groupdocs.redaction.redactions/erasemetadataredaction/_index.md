---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.redaction.redactions/erasemetadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.MetadataRedaction](../../com.groupdocs.redaction.redactions/metadataredaction)
```
public class EraseMetadataRedaction extends MetadataRedaction
```

表示一种元数据编辑，它从文档中擦除所有元数据或匹配特定 MetadataFilters 的元数据。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />

以下示例演示如何擦除（设为空值）全部或特定的元数据。

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

