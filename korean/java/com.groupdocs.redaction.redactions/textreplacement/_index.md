---
title: "TextReplacement"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "텍스트 교체 정보를 나타냅니다."
type: docs
weight: 33
url: /ko/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

텍스트 교체 정보를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | TextReplacement 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getIndex()](#getIndex--) | 소스 문자열 내에서 일치하는 텍스트의 인덱스를 가져옵니다. |
|
|  | [getOriginalText()](#getOriginalText--) | 원래 일치한 문자열을 가져옵니다. |
|
|  | [getReplacement()](#getReplacement--) | OriginalText를 교체한 문자열을 가져옵니다. |
|
|  | [toString()](#toString--) | 텍스트 교체 설명과 해당 위치를 제공합니다. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


TextReplacement 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 원본 문자열 내에서 일치하는 텍스트의 인덱스 |
|
|  | 원본 | java.lang.String | 원래 일치 문자열 |
|
|  | 대체 | java.lang.String | 원본 문자열에서 OriginalText를 교체한 문자열 |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


소스 문자열 내에서 일치하는 텍스트의 인덱스를 가져옵니다.


**Returns:**
int - 원본 문자열 내에서 일치하는 텍스트의 인덱스.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


원래 일치한 문자열을 가져옵니다.


**Returns:**
java.lang.String - 원래 일치 문자열.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


OriginalText를 교체한 문자열을 가져옵니다.


**Returns:**
java.lang.String - OriginalText를 교체한 문자열.

### toString() {#toString--}
```
public String toString()
```


텍스트 교체 설명과 해당 위치를 제공합니다.


**Returns:**
java.lang.String - 교체 설명

