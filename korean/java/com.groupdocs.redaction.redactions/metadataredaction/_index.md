---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서 메타데이터 삭제를 위한 기본 추상 클래스를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

문서 메타데이터 삭제를 위한 기본 추상 클래스를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFilter()](#getFilter--) | 모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터를 가져옵니다. |
|
|  | [setFilter(int value)](#setFilter-int-) | 모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터를 설정합니다. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | 주어진 형식 인스턴스에 레드액션을 적용합니다. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터를 가져옵니다.


**Returns:**
int - 모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | 모든 메타데이터 또는 특정 메타데이터(예: Author 또는 Company)를 선택하는 데 사용되는 필터. |
|

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

