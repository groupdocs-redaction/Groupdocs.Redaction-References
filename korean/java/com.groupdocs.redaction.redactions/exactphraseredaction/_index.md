---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "기본적으로 대소문자를 구분하지 않고 문서 텍스트에서 정확한 구문을 교체하는 텍스트 가리기를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

문서 텍스트에서 정확한 구문을 교체하는 텍스트 Redaction을 나타냅니다. 기본적으로 대소문자를 구분하지 않습니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

다음 예제는 대소문자 구분 구문 검색 및 교체 수행을 보여줍니다.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// 기본적으로, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red))));
doc.save();
}
 
``` 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | 대소문자를 구분하지 않는 모드에서 ExactPhraseRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | ExactPhraseRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | 검색 및 교체할 문자열을 가져옵니다. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | 검색이 대소문자를 구분하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [isRightToLeft()](#isRightToLeft--) | 이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값을 가져옵니다(기본값은 false). |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | 이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값을 설정합니다(기본값은 false). |
|
|  | [getDescription()](#getDescription--) | 레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 주어진 형식 인스턴스에 레드액션을 적용합니다. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


대소문자를 구분하지 않는 모드에서 ExactPhraseRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 검색 및 교체할 문자열 |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 교체 옵션 (텍스트, 색상) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


ExactPhraseRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | 검색 및 교체할 문자열 |
|
|  | isCaseSensitive | boolean | 대소문자 구분 검색이 필요한 경우 true |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | 교체 옵션 (텍스트, 색상) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


검색 및 교체할 문자열을 가져옵니다.


**Returns:**
java.lang.String - 검색 및 교체할 문자열.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


검색이 대소문자를 구분하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 검색이 대소문자를 구분하는지 여부를 나타내는 값.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값을 가져옵니다(기본값은 false).


**Returns:**
boolean - 이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값(기본값은 false).

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값을 설정합니다(기본값은 false).


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 이 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 값(기본값은 false). |
|

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

