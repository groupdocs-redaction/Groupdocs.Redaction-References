---
title: "IReleasePageStream"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en metod som frigör strömmen som skapats av delegaten CreatePageStream."
type: docs
weight: 18
url: /sv/java/com.groupdocs.redaction.options/ireleasepagestream/
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

