---
title: ITextualFormatInstance
second_title: GroupDocs.Redaction for Java API Reference
description: Defines methods that are required for redacting textual data in any document containing text.
type: docs
weight: 28
url: /java/com.groupdocs.redaction.integration/itextualformatinstance/
---```
public interface ITextualFormatInstance
```

Defines methods that are required for redacting textual data in any document, containing text.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document text redactions: [Text redactions][]
 *  More details about implementing custom formats: [Create custom format handler][]


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Text redactions]: https://docs.groupdocs.com/redaction/java/text-redactions/
[Create custom format handler]: https://docs.groupdocs.com/redaction/java/create-custom-format-handler/
## Methods

| Method | Description |
| --- | --- |
| [replaceText(Pattern regularExpression, ReplacementOptions options)](#replaceText-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Replaces all matches of the regular expression with a given replacement. |
### replaceText(Pattern regularExpression, ReplacementOptions options) {#replaceText-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public abstract RedactionResult replaceText(Pattern regularExpression, ReplacementOptions options)
```


Replaces all matches of the regular expression with a given replacement.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | allow to set textual replacement or color for redaction block |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Text replacement result
