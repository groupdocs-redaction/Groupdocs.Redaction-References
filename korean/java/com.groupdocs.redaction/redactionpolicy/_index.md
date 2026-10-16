---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "적용할 특정 편집 집합을 포함하는 정화 정책을 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

적용할 특정 가림 처리 집합을 포함하는 정화 정책을 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | 새 Redaction 정책 인스턴스를 생성합니다. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | 특정 편집 목록을 사용하여 새 Redaction 정책 인스턴스를 생성합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | 완전히 구성된 배열을 가져옵니다 |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | 인스턴스를 로드합니다 |
RedactionPolicy
파일 경로에서.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | 인스턴스를 로드합니다 |
RedactionPolicy
스트림에서.
|
|  | [save(String filePath)](#save-java.lang.String-) | redaction 정책을 파일에 저장합니다. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | redaction 정책을 스트림에 저장합니다. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


새 Redaction 정책 인스턴스를 생성합니다.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


특정 편집 목록을 사용하여 새 Redaction 정책 인스턴스를 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | 정책에 대한 편집 배열 |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


완전히 구성된 배열을 가져옵니다
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - 완전히 구성된 Redaction 파생 클래스 배열.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


인스턴스를 로드합니다
RedactionPolicy
파일 경로에서.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | XML 파일 경로 |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


인스턴스를 로드합니다
RedactionPolicy
스트림에서.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 입력 | java.io.InputStream | XML 구성을 포함하는 스트림 |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


redaction 정책을 파일에 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


redaction 정책을 스트림에 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 정책을 저장할 대상 스트림 |
|

