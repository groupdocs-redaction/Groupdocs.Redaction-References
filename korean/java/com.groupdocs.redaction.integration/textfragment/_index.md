---
title: "TextFragment"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "OCR 엔진에 의해 추출된 인식된 텍스트, 단어, 기호 등의 일부를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

OCR 엔진에 의해 추출된 인식된 텍스트(단어, 기호 등)의 일부를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | 인식된 텍스트 조각의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getText()](#getText--) | 인식된 텍스트 조각의 텍스트 내용을 가져옵니다. |
|
|  | [getRectangle()](#getRectangle--) | 인식된 텍스트 조각의 경계 사각형을 가져옵니다. |
|
|  | [toString()](#toString--) | 인식된 텍스트 조각의 텍스트 내용을 반환합니다. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


인식된 텍스트 조각의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 텍스트 | java.lang.String | 인식된 텍스트 조각의 텍스트 내용 |
|
|  | 사각형 | java.awt.Rectangle | 인식된 텍스트 조각의 경계 사각형 |
|

### getText() {#getText--}
```
public final String getText()
```


인식된 텍스트 조각의 텍스트 내용을 가져옵니다.


**Returns:**
java.lang.String - 인식된 텍스트 조각의 텍스트 내용.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


인식된 텍스트 조각의 경계 사각형을 가져옵니다.


**Returns:**
java.awt.Rectangle - 인식된 텍스트 조각의 경계 사각형.

### toString() {#toString--}
```
public String toString()
```


인식된 텍스트 조각의 텍스트 내용을 반환합니다.


**Returns:**
java.lang.String - 인식된 텍스트 조각의 텍스트 내용

