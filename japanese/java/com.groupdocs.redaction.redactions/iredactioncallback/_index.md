---
title: "IRedactionCallback"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "各削除変更に関する情報を受け取り、必要に応じてそれを防止するために必要なメソッドを定義します。"
type: docs
weight: 35
url: /ja/java/com.groupdocs.redaction.redactions/iredactioncallback/
---```
public interface IRedactionCallback
```

Defines methods that are required for receiving information on each redaction change and optionally prevent it.

*** ** * ** ***


**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [acceptRedaction(RedactionDescription description)](#acceptRedaction-com.groupdocs.redaction.redactions.RedactionDescription-) | This call is triggered right before applying any redaction to the document and allows to log or forbid it.
 |
### acceptRedaction(RedactionDescription description) {#acceptRedaction-com.groupdocs.redaction.redactions.RedactionDescription-}
```
public abstract boolean acceptRedaction(RedactionDescription description)
```


This call is triggered right before applying any redaction to the document and allows to log or forbid it.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| description | [RedactionDescription](../../com.groupdocs.redaction.redactions/redactiondescription) | Contains information about particular match type, criteria, text and position
 |

**Returns:**
boolean - Return true to accept or false to decline particular match redaction

