---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 삭제를 나타냅니다."
type: docs
weight: 28
url: /ko/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 삭제를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | RegexRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | 일치시킬 정규 표현식을 가져옵니다. |
|
|  | [getDescription()](#getDescription--) | 레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 주어진 형식 인스턴스에 레드액션을 적용합니다. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


RegexRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 패턴 | java.lang.String | 검색 및 교체를 위한 정규식 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 교체 옵션 (텍스트, 색상) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


RegexRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 정규식 | java.util.regex.Pattern | 검색 및 교체를 위한 정규식 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 교체 옵션 (텍스트, 색상) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


일치시킬 정규 표현식을 가져옵니다.


**Returns:**
java.util.regex.Pattern - 일치시킬 정규식.

### getDescription() {#getDescription--}
```
public String getDescription()
```


레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다.


**Returns:**
java.lang.String - 레드액션 이름 및 매개변수를 포함하는 텍스트.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


주어진 형식 인스턴스에 레드액션을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 레드액션을 적용할 문서 인스턴스 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

