---
title: "Redactor"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "문서 레드랙션 프로세스를 제어하고 문서를 열고 레드랙션하고 저장할 수 있게 하는 주요 클래스를 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

문서 가림 처리 프로세스를 제어하는 주요 클래스를 나타내며, 문서를 열고, 가림 처리하고, 저장할 수 있게 합니다.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | 새 인스턴스를 초기화합니다. |
Redactor
파일 경로를 사용하는 클래스.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | 새 인스턴스를 초기화합니다. |
Redactor
스트림을 사용하는 클래스.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | 새 인스턴스를 초기화합니다. |
Redactor
경로를 사용하여 암호 보호된 문서에 대한 클래스.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 새 인스턴스를 초기화합니다. |
Redactor
경로와 설정을 사용하여 암호 보호된 문서에 대한 클래스.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | 새 인스턴스를 초기화합니다. |
Redactor
스트림을 사용하여 암호 보호된 문서에 대한 클래스.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | 새 인스턴스를 초기화합니다. |
Redactor
스트림과 설정을 사용하여 암호 보호된 문서에 대한 클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [close()](#close--) | 리소스를 해제합니다. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | 문서에 레드랙션을 적용합니다. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | 문서에 일련의 레드랙션을 적용합니다. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | 문서에 레드랙션 정책을 적용합니다. |
|
|  | [save()](#save--) | 다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | 문서를 파일에 저장합니다. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | 문서를 스트림에 저장합니다. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | 문서를 스트림에 저장합니다. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | 문서를 스트림에 저장하고 사용자 지정 위치를 포함합니다. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | 지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | 문서에 대한 일반 정보(크기, 페이지 수 등)를 가져옵니다. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


새 인스턴스를 초기화합니다.
Redactor
파일 경로를 사용하는 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로 |


다음 예제는 레드랙션을 위해 문서를 여는 방법을 보여줍니다.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// 여기에서 document 인스턴스를 사용하여 redaction을 수행할 수 있습니다
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


새 인스턴스를 초기화합니다.
Redactor
경로를 사용하여 암호 보호된 문서에 대한 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 옵션, 비밀번호 포함. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


새 인스턴스를 초기화합니다.
Redactor
경로와 설정을 사용하여 암호 보호된 문서에 대한 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 파일 종속 옵션, 비밀번호 포함. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | redaction 프로세스에 대한 기본 설정. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


새 인스턴스를 초기화합니다.
Redactor
스트림을 사용하여 암호 보호된 문서에 대한 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | document | java.io.InputStream | 소스 입력 스트림. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 옵션, 비밀번호 포함. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


새 인스턴스를 초기화합니다.
Redactor
스트림과 설정을 사용하여 암호 보호된 문서에 대한 클래스.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | document | java.io.InputStream | 소스 입력 스트림. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | 옵션, 비밀번호 포함. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | redaction 프로세스에 대한 기본 설정. |
|

### close() {#close--}
```
public final void close()
```


리소스를 해제합니다.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


문서에 레드랙션을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | 적용할 Redaction 인스턴스 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


문서에 일련의 레드랙션을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | 적용할 redactions 배열 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


문서에 레드랙션 정책을 적용합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redaction 정책 |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


다음 옵션을 사용하여 문서를 파일에 저장합니다: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - redacted 문서 경로

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


문서를 파일에 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | 접미사를 추가하거나 rasterize 하는 옵션 |
|

**Returns:**
java.lang.String - redacted 문서 경로

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


문서를 스트림에 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | document | java.io.OutputStream | 대상 스트림 |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


문서를 스트림에 저장합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | document | java.io.OutputStream | 대상 스트림 |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | 저장 옵션 |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


문서를 스트림에 저장하고 사용자 지정 위치를 포함합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | document | java.io.OutputStream | 대상 스트림 |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | rasterize 여부와 rasterization 페이지를 지정하는 옵션 |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


지정된 이미지 형식으로 특정 페이지의 미리보기 이미지를 생성합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | 이미지 속성 및 페이지 범위 설정 |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


문서에 대한 일반 정보(크기, 페이지 수 등)를 가져옵니다.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

