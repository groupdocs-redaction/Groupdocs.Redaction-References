---
title: "ICreatePageStream"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "페이지 미리보기 데이터를 쓰기 위한 스트림을 반환하는 메서드를 제공합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.redaction.options/icreatepagestream/
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

