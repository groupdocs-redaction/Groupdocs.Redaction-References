---
title: "Redaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "모든 가림 처리 유형에 대한 기본 추상 클래스를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

모든 가림 처리 유형에 대한 기본 추상 클래스를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDescription()](#getDescription--) | 레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 주어진 형식 인스턴스에 레드액션을 적용합니다. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


레드액션 및 해당 매개변수를 설명하는 문자열을 반환합니다.


**Returns:**
java.lang.String - 레드액션 이름 및 매개변수를 포함하는 텍스트.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


주어진 형식 인스턴스에 레드액션을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | 레드액션을 적용할 문서 인스턴스 |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

