---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "출력 파일 이름을 변경하거나 문서를 이미지 기반 PDF 래스터화로 변환하기 위한 옵션을 제공합니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

출력 파일 이름을 변경하고/또는 문서를 이미지 기반 PDF(래스터화)로 변환하는 옵션을 제공합니다.

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | 새 인스턴스를 기본값으로 초기화합니다: PDF로 래스터화 - false, 접미사 추가 - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | 주어진 매개변수로 새 인스턴스를 초기화합니다. |
|
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | 기본 접미사 값인 "Redacted"를 나타냅니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | 저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | 저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | 출력 파일 이름에 대한 사용자 지정 접미사를 가져옵니다. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | 출력 파일 이름에 대한 사용자 지정 접미사를 설정합니다. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getRasterization()](#getRasterization--) | 래스터화 설정을 가져옵니다. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | 워드 프로세싱 저장 옵션. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


새 인스턴스를 기본값으로 초기화합니다: PDF로 래스터화 - false, 접미사 추가 - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


주어진 매개변수로 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는 경우 True |
|
|  | suffix | java.lang.String | 이 텍스트는 파일 이름 끝에 추가되며, 비어 있지 않은 경우 AddSuffix를 true로 설정합니다. |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


기본 접미사 값인 "Redacted"를 나타냅니다.


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값을 가져옵니다. 기본값은 False입니다.


**Returns:**
boolean - 저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값입니다. 기본값은 False입니다.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값을 설정합니다. 기본값은 False입니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 저장하기 전에 파일 이름을 변경해야 하는지 여부를 나타내는 값입니다. 기본값은 False입니다. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


출력 파일 이름에 대한 사용자 지정 접미사를 가져옵니다. 지정되지 않은 경우,
SaveSuffix
상수가 사용됩니다.


**Returns:**
java.lang.String - 출력 파일 이름에 대한 사용자 지정 접미사입니다. 지정되지 않은 경우,  SaveSuffix  상수가 사용됩니다.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


출력 파일 이름에 대한 사용자 지정 접미사를 설정합니다. 지정되지 않은 경우,
SaveSuffix
상수가 사용됩니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 출력 파일 이름에 대한 사용자 지정 접미사입니다. 지정되지 않은 경우 SaveSuffix 상수가 사용됩니다. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지를 나타내는 값입니다.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지 여부를 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 문서의 모든 페이지를 이미지로 변환하여 단일 PDF 파일에 넣어야 하는지를 나타내는 값입니다. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


래스터화 설정을 가져옵니다.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


워드 프로세싱 저장 옵션.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
