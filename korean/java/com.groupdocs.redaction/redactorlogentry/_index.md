---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "가림 처리 적용 결과를 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

가림 처리 적용 결과를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | 편집을 위해 RedactorLogEntry 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getResult()](#getResult--) | 반환된 결과를 가져옵니다. |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | 레드랙션에 대한 참조와 해당 옵션을 가져옵니다. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


편집을 위해 RedactorLogEntry 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | 레드랙션에 대한 참조 |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | 포맷 핸들러가 보고한 레드랙션 결과 |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


반환된 결과를 가져옵니다.
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


레드랙션에 대한 참조와 해당 옵션을 가져옵니다.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

