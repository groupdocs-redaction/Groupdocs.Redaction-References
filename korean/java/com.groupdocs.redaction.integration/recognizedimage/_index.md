---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "인식 프로세스 결과 이미지에서 추출된 텍스트를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

이미지에서 인식 과정을 통해 추출된 텍스트를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | 인식된 라인의 집합을 사용하여 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getText()](#getText--) | 구조화된 텍스트의 텍스트 등가물을 가져옵니다. |
|
|  | [getLines()](#getLines--) | 문서 내에서 인식된 텍스트 라인과 해당 조각들을 가져옵니다. |
|
|  | [toString()](#toString--) | 구조화된 텍스트의 텍스트 등가물을 가져옵니다. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


인식된 라인의 집합을 사용하여 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | 인식된 라인의 IEnumerable(예: 리스트 또는 배열) |
|

### getText() {#getText--}
```
public final String getText()
```


구조화된 텍스트의 텍스트 등가물을 가져옵니다.


**Returns:**
java.lang.String - 구조화된 텍스트의 텍스트 등가물.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


문서 내에서 인식된 텍스트 라인과 해당 조각들을 가져옵니다.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - 문서 내에서 인식된 텍스트 라인과 해당 조각들.

### toString() {#toString--}
```
public String toString()
```


구조화된 텍스트의 텍스트 등가물을 가져옵니다.


**Returns:**
java.lang.String - 인식된 텍스트

