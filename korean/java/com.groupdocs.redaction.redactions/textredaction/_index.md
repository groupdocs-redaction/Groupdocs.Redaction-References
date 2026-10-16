---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서 텍스트 삭제를 위한 기본 추상 클래스를 나타냅니다."
type: docs
weight: 32
url: /ko/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

문서 텍스트 삭제를 위한 기본 추상 클래스를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | 가져옵니다 |
ReplacementOptions
인스턴스, 텍스트 교체 유형을 지정합니다.
|
|  | [getOcrConnector()](#getOcrConnector--) | 가져옵니다 |
IOcrConnector
구현, 그래픽 콘텐츠에서 텍스트를 추출하는 데 필요합니다.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 설정합니다 |
IOcrConnector
구현, 그래픽 콘텐츠에서 텍스트를 추출하는 데 필요합니다.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


가져옵니다
ReplacementOptions
인스턴스, 텍스트 교체 유형을 지정합니다.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


가져옵니다
IOcrConnector
구현, 그래픽 콘텐츠에서 텍스트를 추출하는 데 필요합니다.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


설정합니다
IOcrConnector
구현, 그래픽 콘텐츠에서 텍스트를 추출하는 데 필요합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector 구현, 그래픽 콘텐츠에서 텍스트를 추출하는 데 필요합니다. |
|

