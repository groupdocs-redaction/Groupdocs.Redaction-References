---
title: ICustomRedactionHandler
second_title: GroupDocs.Redaction for Java API Reference
description: Defines a custom redaction callback.
type: docs
weight: 34
url: /java/com.groupdocs.redaction.redactions/icustomredactionhandler/
---```
public interface ICustomRedactionHandler
```

Defines a custom redaction callback. Currently supported for PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) only.

## Methods

| Method | Description |
| --- | --- |
| [redact(CustomRedactionContext context)](#redact-com.groupdocs.redaction.redactions.CustomRedactionContext-) | Processes a matched text fragment and returns redaction decision.
 |
### redact(CustomRedactionContext context) {#redact-com.groupdocs.redaction.redactions.CustomRedactionContext-}
```
public abstract CustomRedactionResult redact(CustomRedactionContext context)
```


Processes a matched text fragment and returns redaction decision.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| context | com.groupdocs.redaction.redactions.CustomRedactionContext | Matched fragment information.
 |

**Returns:**
[CustomRedactionResult](../../com.groupdocs.redaction.redactions/customredactionresult) - Redaction decision and optional replacement text.

