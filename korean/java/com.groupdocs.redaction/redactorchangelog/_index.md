---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "Redactor 클래스의 Apply 메서드에 전달된 일괄 편집 결과 목록을 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Apply() 메서드에 전달된 일괄 편집 결과 목록을 나타냅니다,
Redactor
클래스.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | RedactorChangeLog 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 적용된 모든 일괄 편집의 최종 상태를 가져옵니다. |
|
|  | [getRedactionLog()](#getRedactionLog--) | 목록을 가져옵니다 |
RedactorLogEntry
인스턴스.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


RedactorChangeLog 클래스의 새 인스턴스를 초기화합니다.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


적용된 모든 일괄 편집의 최종 상태를 가져옵니다.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


목록을 가져옵니다
RedactorLogEntry
인스턴스.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - RedactorLogEntry 인스턴스 목록.

