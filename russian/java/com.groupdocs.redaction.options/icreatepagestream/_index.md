---
title: "ICreatePageStream"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет метод, возвращающий поток для записи данных предварительного просмотра страниц."
type: docs
weight: 16
url: /ru/java/com.groupdocs.redaction.options/icreatepagestream/
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

