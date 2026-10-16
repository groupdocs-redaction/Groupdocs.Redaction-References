---
title: "ITextualFormatInstance"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "텍스트를 포함하는 모든 문서에서 텍스트 데이터를 편집하기 위해 필요한 메서드를 정의합니다."
type: docs
weight: 27
url: /ko/java/com.groupdocs.redaction.integration/itextualformatinstance/
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

