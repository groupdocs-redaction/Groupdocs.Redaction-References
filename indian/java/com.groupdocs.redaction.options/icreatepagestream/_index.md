---
title: "ICreatePageStream"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "एक मेथड प्रदान करता है जो पेज प्रीव्यू डेटा लिखने के लिए स्ट्रीम लौटाता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.redaction.options/icreatepagestream/
---```
public interface ICreatePageStream
```

Provides method that returns a stream to write page preview data.

## Methods

| Method | Description |
| --- | --- |
| [createPageStream(int pageNumber)](#createPageStream-int-) | Represents method that returns a stream to write page preview data.
 |
### createPageStream(int pageNumber) {#createPageStream-int-}
```
public abstract OutputStream createPageStream(int pageNumber)
```


Represents method that returns a stream to write page preview data.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | Page number of a page to generate thumbnail
 |

**Returns:**
java.io.OutputStream - Stream to write page preview

