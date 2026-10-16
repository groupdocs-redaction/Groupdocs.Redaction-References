---
title: "TextLine"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "이미지에서 OCR 엔진으로 추출된 텍스트 라인을 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

이미지에서 OCR 엔진이 추출한 텍스트 라인을 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | 이미지에서 OCR 엔진으로 추출된 텍스트 라인의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFragments()](#getFragments--) | 라인에서 인식된 기호 및 단어와 같은 텍스트 조각 배열을 가져옵니다. |
|
|  | [toString()](#toString--) | 인식된 텍스트 라인의 텍스트 내용을 반환합니다. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


이미지에서 OCR 엔진으로 추출된 텍스트 라인의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | 초기 텍스트 조각 집합 |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


라인에서 인식된 기호 및 단어와 같은 텍스트 조각 배열을 가져옵니다.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - 라인에서 인식된 기호 및 단어와 같은 텍스트 조각 배열.

### toString() {#toString--}
```
public String toString()
```


인식된 텍스트 라인의 텍스트 내용을 반환합니다.


**Returns:**
java.lang.String - 인식된 텍스트 라인의 텍스트 내용

