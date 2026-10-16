---
title: "ITextualFormatInstance"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Define los métodos requeridos para redactar datos textuales en cualquier documento que contenga texto."
type: docs
weight: 27
url: /es/java/com.groupdocs.redaction.integration/itextualformatinstance/
---```
public interface ITextualFormatInstance
```

Defines methods that are required for redacting textual data in any document, containing text.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about implementing custom formats: [Create custom format handler](../https://docs.groupdocs.com/redaction/java/create-custom-format-handler/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [replaceText(Pattern regularExpression, ReplacementOptions options)](#replaceText-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Replaces all matches of the regular expression with a given replacement.
 |
### replaceText(Pattern regularExpression, ReplacementOptions options) {#replaceText-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public abstract RedactionResult replaceText(Pattern regularExpression, ReplacementOptions options)
```


Replaces all matches of the regular expression with a given replacement.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace
 |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | allow to set textual replacement or color for redaction block
 |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Text replacement result

