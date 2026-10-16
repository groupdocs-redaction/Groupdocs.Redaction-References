---
title: "EraseMetadataRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 Redaction을 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.redaction.redactions/erasemetadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.MetadataRedaction](../../com.groupdocs.redaction.redactions/metadataredaction)
```
public class EraseMetadataRedaction extends MetadataRedaction
```

문서에서 모든 메타데이터 또는 특정 MetadataFilters와 일치하는 메타데이터를 지우는 메타데이터 Redaction을 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />

다음 예제는 모든 메타데이터 또는 특정 메타데이터를 지우는(빈 값으로 설정하는) 방법을 보여줍니다.

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

