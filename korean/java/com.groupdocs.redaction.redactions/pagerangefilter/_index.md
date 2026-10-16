---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서 내에서 레드랙션을 적용하기 위해 페이지 범위를 설정하는 레드랙션 필터를 나타냅니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

문서 내에서 삭제를 적용할 페이지 범위를 설정하는 삭제 필터를 나타냅니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | RemovePageRedaction 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | 문서의 시작 또는 끝인 탐색 기준 위치를 가져옵니다. |
|
|  | [getIndex()](#getIndex--) | 시작 위치 인덱스(0부터 시작)를 가져옵니다. |
|
|  | [getCount()](#getCount--) | 제거할 페이지 수를 가져옵니다. |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | 이 필터 페이지 범위에 지정된 페이지가 포함되는지 확인합니다. |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


RemovePageRedaction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | 문서의 시작 또는 끝인 탐색 기준 위치 |
|
|  | 인덱스 | int | 시작 위치 인덱스(0부터 시작) |
|
|  | 개수 | int | 제거할 페이지 수 |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


문서의 시작 또는 끝인 탐색 기준 위치를 가져옵니다.


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


시작 위치 인덱스(0부터 시작)를 가져옵니다.


**Returns:**
int - 시작 위치 인덱스 (0 기반).

### getCount() {#getCount--}
```
public final int getCount()
```


제거할 페이지 수를 가져옵니다.


**Returns:**
int - 제거할 페이지 수.

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


이 필터 페이지 범위에 지정된 페이지가 포함되는지 확인합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | pageIndex | int | 페이지 인덱스 (0 기반) |
|
|  | pageCount | int | 전체 페이지 수 |
|

**Returns:**
boolean - 이 필터 범위에 페이지가 포함된 경우 true

