---
title: "IReleasePageStream"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "CreatePageStream デリゲートによって作成されたストリームを解放するメソッドを表します。"
type: docs
weight: 18
url: /ja/java/com.groupdocs.redaction.options/ireleasepagestream/
---```
public interface IReleasePageStream
```

Represents a method which releases stream created by 
CreatePageStream
 delegate.

## Methods

| Method | Description |
| --- | --- |
| [releasePageStream(int pageNumber, OutputStream pageStream)](#releasePageStream-int-java.io.OutputStream-) | Represents a method which releases stream created by 
CreatePageStream
 delegate.
 |
### releasePageStream(int pageNumber, OutputStream pageStream) {#releasePageStream-int-java.io.OutputStream-}
```
public abstract void releasePageStream(int pageNumber, OutputStream pageStream)
```


Represents a method which releases stream created by 
CreatePageStream
 delegate.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | Page number of the generated page preview
 |
| pageStream | java.io.OutputStream | Stream, containing the generated page preview
 |

