---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "파일을 PDF로 변환하기 위한 옵션을 제공합니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

파일을 PDF로 변환하기 위한 옵션을 제공합니다.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getPageIndex()](#getPageIndex--) | PDF로 변환할 첫 번째 페이지(0 기반)의 인덱스를 가져옵니다. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | PDF로 변환할 첫 번째 페이지(0 기반)의 인덱스를 설정합니다. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | 초기화 후 PageIndex 속성이 변경(설정)되었는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getPageCount()](#getPageCount--) | PDF로 변환될 페이지 수를 가져옵니다. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | PDF로 변환될 페이지 수를 설정합니다. |
|
|  | [isPageCountSet()](#isPageCountSet--) | 초기화 후 PageCount 속성이 변경(설정)되었는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getCompliance()](#getCompliance--) | PDF 준수 수준을 가져옵니다. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | PDF 준수 수준을 설정합니다. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | 고급 래스터화 옵션이 설정된 경우 true인 표시기를 가져옵니다. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | 이 메서드를 사용하여 적용할 고급 래스터화 옵션을 등록할 수 있습니다. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | 이 메서드를 사용하여 적용할 고급 래스터화 옵션을 등록할 수 있습니다. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


새 인스턴스를 초기화합니다.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 가져옵니다. 기본값은 TRUE이며, 래스터화를 방지하려면 FALSE로 설정합니다.


**Returns:**
boolean - 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값. 기본값은 TRUE이며, 래스터화를 방지하려면 FALSE로 설정합니다.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 설정합니다. 기본값은 TRUE이며, 래스터화를 방지하려면 FALSE로 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값. 기본값은 TRUE이며, 래스터화를 방지하려면 FALSE로 설정합니다. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


PDF로 변환할 첫 번째 페이지(0 기반)의 인덱스를 가져옵니다.


**Returns:**
int - PDF로 변환할 첫 번째 페이지(0부터 시작)의 인덱스.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


PDF로 변환할 첫 번째 페이지(0 기반)의 인덱스를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | PDF로 변환할 첫 번째 페이지(0부터 시작)의 인덱스. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


초기화 후 PageIndex 속성이 변경(설정)되었는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 초기화 후 PageIndex 속성이 변경(설정)되었는지 여부를 나타내는 값.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


PDF로 변환될 페이지 수를 가져옵니다.


**Returns:**
int - PDF로 변환될 페이지 수.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


PDF로 변환될 페이지 수를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | int | PDF로 변환될 페이지 수. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


초기화 후 PageCount 속성이 변경(설정)되었는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 초기화 후 PageCount 속성이 변경(설정)되었는지 여부를 나타내는 값.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


PDF 준수 수준을 가져옵니다.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


PDF 준수 수준을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF 준수 수준. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


고급 래스터화 옵션이 설정된 경우 true인 표시기를 가져옵니다.


**Returns:**
boolean - 고급 래스터화 옵션이 설정된 경우 true인 표시기.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


이 메서드를 사용하여 적용할 고급 래스터화 옵션을 등록할 수 있습니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 선택된 효과 유형(그레이스케일, 테두리 등)에 대한 정보를 제공합니다. |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


이 메서드를 사용하여 적용할 고급 래스터화 옵션을 등록할 수 있습니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | 선택된 효과 유형(그레이스케일, 테두리 등)에 대한 정보를 제공합니다. |
|
|  | 매개변수 | java.util.HashMap<java.lang.String,java.lang.String> | 회전 각도와 같은 지정된 효과에 대한 매개변수 |
|

